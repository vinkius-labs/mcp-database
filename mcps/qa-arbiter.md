# QA Arbiter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qa-arbiter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A test fails. Is the assertion wrong or is the code broken? Most agents guess, retry blindly, and deadlock the pipeline. QA Arbiter resolves this in one call — structured fault diagnosis with two boolean pivots that yield a deterministic verdict: TEST_ERROR, ENGINE_DEFECT, or BOTH_WRONG.

## Description
When a QA agent sees a failing test, it faces a critical question: **is the test wrong, or is the code broken?** Most agents skip this question entirely — they guess, retry blindly, or blame the wrong component. QA Arbiter eliminates this failure mode.

### The Problem It Solves

In multi-agent pipelines, QA agents write tests and run them. When tests fail, two things can be true:

1. **The test's expected value is wrong** — the agent miscalculated (e.g., wrote `'05:25'` instead of `'04:45'`).
2. **The engine has a real bug** — the code produces incorrect output (e.g., `-02:-15` from a midnight crossover bug).

Without structured diagnosis, agents waste cycles: QA blames the developer → developer can't fix test code → pipeline deadlocks.

### How It Works

QA Arbiter uses the **Decision Pivot** pattern from reasoning research. For each failing test, the agent must call this tool and fill in structured fields:

1. **Trace** the engine function step-by-step with the test's inputs.
2. **Compare** the vitest `Received` value against the trace.
3. **Compare** the test's `Expected` value against the trace.
4. **Commit** to two boolean pivots: `receivedMatchesTrace` and `expectedMatchesTrace`.
5. The **verdict** follows deterministically from the pivots.

The tool **validates logical consistency** — if the agent says `ENGINE_DEFECT` but marked `receivedMatchesTrace: true`, the tool rejects the diagnosis with a clear explanation of the contradiction. The agent must re-analyze.

### Why It Works

- **Tool calls are obligations, instructions are suggestions.** Agents routinely ignore prompt instructions to "check your work." A tool call cannot be skipped — the agent must fill every field.
- **Decision Pivots eliminate guesswork.** Two booleans + consistency validation = deterministic verdict. The agent cannot arrive at a wrong conclusion without contradicting itself.
- **Zero computation.** The tool doesn't calculate anything. It forces the agent to show its reasoning, then validates that the reasoning is internally consistent.


## Available Tools (1)
- **diagnose_test_failure**: You must: (1) TRACE the engine function step-by-step with the EXACT test inputs — show every intermediate calculation, every branch taken, every value produced. No hand-waving ("it processes the data") — arithmetic, values, intermediate results, (2) COMPARE vitest "Received" against your trace — if Received matches your trace, the engine is doing what it is designed to do, (3) COMPARE vitest "Expected" (what the test asserts) against your trace — if Expected does NOT match your trace, the test author made an error, (4) The VERDICT follows deterministically from the two PIVOTs: Received=Trace AND Expected≠Trace → TEST_ERROR. Received≠Trace AND Expected=Trace → ENGINE_DEFECT. Received≠Trace AND Expected≠Trace → BOTH_WRONG. Received=Trace AND Expected=Trace → FALSE_ALARM (investigate assertion comparison). If the tool rejects, your trace has a gap — re-examine the intermediate calculations.

Structured diagnostic for failing tests — forces deterministic, step-by-step root cause analysis that separates test errors from genuine engine defects before any code is changed. Based on the Decision Pivot pattern from ROMA (2024) and the scientific debugging method (Zeller, "Why Programs Fail", 2009). Catches Assertion Confusion (the test asserts the wrong expected value — test: "calculateTax(100, 0.08) should return 108." Received: 8. Expected (from test): 108. The test author confused total-with-tax (100 + 8 = 108) with tax-amount (100 × 0.08 = 8). The engine is correct — it returns the tax, not the total. The test is wrong. Without systematic tracing, the developer "fixes" the engine to return 108, breaking every downstream consumer that depends on receiving the tax amount. This is the #1 cause of "fix introduces regression" — the test was wrong, not the code. The trace proves it: fn(100, 0.08) → 100 × 0.08 = 8.00. Received=8 matches trace. Expected=108 does NOT match trace. Verdict: TEST_ERROR), Environment Pollution (test passes in isolation but fails in suite due to shared state — Test A sets global config: config.taxRate = 0.10. Test B assumes default: config.taxRate = 0.08. When run in isolation: Test B passes (default 0.08). When run after Test A: Test B fails (0.10 persists). The test is correct. The engine is correct. The environment is polluted. Symptoms: "works on my machine," "passes when run alone," "fails only in CI." Diagnosis: run the failing test with --run-in-band (sequential). If it fails: engine/test bug. If it passes: environment pollution from another test. Fix: beforeEach/afterEach cleanup, no global state mutation, test isolation with factory functions), Flaky Test Tolerance (accepting intermittent failures as "normal" — "Oh, that test is flaky, just re-run it." A test that fails 5% of the time is a test that PASSES 95% of the time — meaning the bug it catches goes undetected in 19 out of 20 runs. In a CI pipeline running 500 tests, 5% flake rate = 25 flaky tests = team re-runs CI 3-4 times per PR = 45 minutes wasted per PR = 15 hours/week across a 10-person team. Causes: timing dependencies (setTimeout/race conditions), external service calls in tests, shared mutable state, date/time dependencies (test breaks at midnight), random data without seed. Each flaky test must be quarantined, root-caused, and either fixed or deleted — never tolerated), Coverage Theater (high coverage percentage that tests nothing meaningful — "98% code coverage!" But the tests assert: expect(result).toBeDefined(). That is existence testing — it proves the function returns SOMETHING, not the RIGHT thing. Coverage measures lines EXECUTED, not behavior VERIFIED. A test that calls createUser({name: "test"}) and asserts expect(result).toBeTruthy() covers the createUser function but verifies nothing about: validation (does it reject empty names?), uniqueness (does it catch duplicates?), or side effects (does it send the welcome email?). Mutation testing (Stryker) is the antidote: it modifies the code and checks if tests fail. If a mutation survives (code changed but tests still pass), the test is theater), and Regression Blindness (fixing a bug without adding a test that prevents recurrence — "Fixed the off-by-one error in pagination." But no regression test was added. 3 sprints later, a refactor reintroduces the same bug. The team spends 4 hours debugging what they already solved. Rule: every bug fix requires a regression test that REPRODUCES the bug first (red), then proves the fix works (green). The regression test is not just a safety net — it is DOCUMENTATION of the bug, its trigger condition, and the expected behavior after the fix. Without it, the fix is temporary — it will return). Call once per failing test before attempting any fix


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QA Arbiter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a failing test: expected '05:25' but received '04:45'. The engine computes bedtime as wake_time minus (cycles × 90 + 15) minutes. For 2 cycles from 08:00, diagnose this failure."

**🤖 AI Agent:**
> Verdict: TEST_ERROR. Trace: 2×90+15=195min, 480-195=285min → 04:45. The engine correctly returns '04:45'. Your expected value '05:25' is wrong — fix it to '04:45'.

---

**👤 You:**
> "My test expects '22:45' for 6 cycles from 08:00, but the engine returns '-02:-15'. This looks like a midnight crossover bug."

**🤖 AI Agent:**
> Verdict: ENGINE_DEFECT. Trace: 6×90+15=555min, 480-555=-75min → JS modulo gives -2h-15m = '-02:-15' (incorrect). Domain-correct: (-75+1440)%1440=1365min → 22:45. Root cause: JavaScript % operator preserves sign on negative numbers. Keep this test — it documents the bug.

---

**👤 You:**
> "After diagnosing 6 test failures, what is the aggregate recommendation for my QA pipeline?"

**🤖 AI Agent:**
> Session Summary — 6 analyzed: 4 TEST_ERROR, 1 ENGINE_DEFECT, 1 BOTH_WRONG. Recommendation: MIXED. Fix your 4 test assertions first, then report the engine defect with traced proof to the developer agent.


## ❓ FAQ

**Q: Does QA Arbiter run my tests or compute expected values?**
No. QA Arbiter performs zero computation and zero side effects. It forces the AI agent to structure its own reasoning into verifiable steps, then validates that the reasoning is logically consistent. Think of it as a reasoning enforcer — like Sequential Thinking, but specialized for test failure diagnosis.

**Q: What are Decision Pivots?**
Decision Pivots are minimal, verifiable checkpoints that all correct reasoning paths must pass through — a concept from the ROMA research framework. In QA Arbiter, the two pivots are boolean fields: `receivedMatchesTrace` (does the engine's output match the hand-traced computation?) and `expectedMatchesTrace` (does the test's expected value match?). The verdict is derived deterministically from these two booleans, making it impossible to reach a wrong conclusion without contradicting yourself.

**Q: How does it prevent pipeline deadlocks in multi-agent systems?**
In a typical QA→Developer pipeline, when tests fail, the system routes back to the developer. But if the tests themselves are wrong (QA's fault), the developer can't fix them — creating an infinite retry loop. QA Arbiter forces the QA agent to determine fault attribution BEFORE the pipeline routes: if it's TEST_ERROR, the QA agent fixes its own tests; if it's ENGINE_DEFECT, it routes to the developer with traced proof. The aggregate summary tells the orchestrator exactly what to do.

**Q: What happens if the agent lies about the boolean pivots?**
The consistency validation catches direct contradictions — e.g., if the agent says both values match the trace but chose TEST_ERROR instead of FALSE_ALARM, the tool rejects it. For subtler misrepresentations, the `engineTrace` field creates an auditable trail: post-hoc analysis can cross-reference the trace against the actual engine source code. The structured format makes deception mechanically harder than with free-form text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qa-arbiter](https://vinkius.com/mcp/qa-arbiter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QA Arbiter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qa-arbiter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QA Arbiter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qa-arbiter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Critical Thinking Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/critical-thinking-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents accept premises without questioning, analyze from one perspective, cherry-pick evidence, ignore consequences, and present uncertainty as certainty. This tool forces rigor: surface assumptions, apply competing frameworks, weigh counterevidence, trace ripple effects, bound confidence.

## Description
AI agents produce dangerously confident conclusions on complex problems. They accept the problem framing as given, analyze from their default perspective, find evidence that supports their initial hypothesis, solve the immediate question without tracing consequences, and present everything with 100% confidence. This is not reasoning — it's pattern completion.

### The Problem It Solves

AI reasoning on complex problems fails on five axes:

- **Assumption blindness** — "We need to hire more engineers" without questioning whether headcount is actually the bottleneck. The problem framing IS the problem.
- **Mono-perspective** — Analyzes a business decision purely through an economic lens, ignoring behavioral, ethical, and organizational dynamics.
- **Confirmation bias** — Finds 5 data points supporting the conclusion and 0 contradicting it. Not because contradictions don't exist — because it didn't look for them.
- **Scope neglect** — "Automate this process" without tracing what happens to the people who depend on it, the processes that fed into it, or the systems that consumed its output.
- **False precision** — "The best approach is X" without specifying under what conditions, at what confidence level, or what would change the conclusion.

These aren't knowledge gaps. They're **reasoning gaps.** The agent never asks: what am I assuming? What does this look like from the other side? What evidence contradicts me? What happens next? How sure am I really?

### How It Works

Critical Thinking Prover uses 5 Decision Pivots — boolean checkpoints that force the agent to validate its own reasoning before committing to a conclusion:

1. **assumptionsExposed** — Have you identified the HIDDEN assumptions embedded in this problem? Every problem has them.
2. **perspectivesConsidered** — Have you analyzed from MULTIPLE competing frameworks? Not "different angles" — named mental models.
3. **evidenceWeighed** — Have you evaluated evidence FOR and AGAINST with EQUAL rigor? One-sided evidence is confirmation bias.
4. **consequencesMapped** — Have you traced SECOND-ORDER effects? Who loses when this succeeds? What feedback loops emerge?
5. **uncertaintyAcknowledged** — Have you bounded your CONFIDENCE? What would change your conclusion? Under what conditions does it hold?

The tool validates logical consistency. If the agent says `REASONING_PROVEN` but `assumptionsExposed: false`, the tool rejects with coaching. If the evidence is entirely one-sided, it catches confirmation bias. If the conclusion is a platitude like "it depends," it demands a committed position.

### Why It Works

- **Tool calls are obligations, instructions are suggestions.** The agent can ignore "think critically" in a system prompt. It cannot ignore a schema that demands naming hidden assumptions, presenting counterevidence, and bounding confidence.
- **The commit pattern.** The agent proposes its own verdict, then the server validates it against the pivots. Forced commitment deepens reasoning — the agent must actively decide if its thinking is rigorous.
- **Semantic traps.** The engine catches reasoning-specific anti-patterns: non-assumptions ("no hidden assumptions"), vague frameworks ("different angles"), one-sided evidence ("all evidence supports"), shallow consequences ("no side effects"), overconfident bounds ("100% certain"), and platitude conclusions ("it depends", "both sides have merit").
- **Universal domain.** Unlike specialized MCPs, Critical Thinking Prover applies to ANY complex problem — technical architecture, business strategy, policy design, ethical dilemmas, resource allocation, organizational change.


## Available Tools
- **validate_task_completion**: "I think I am done" is not proof. You must: (1) state the OBJECTIVE clearly — what was the user's actual request?, (2) CHECKLIST all requirements from the prompt — each requirement mapped to a specific file change or action taken. Generic "addressed all requirements" is not a checklist, (3) list MODIFIED FILES — exact paths with line ranges. "Updated the code" is not traceability, (4) provide VERIFICATION LOGS — compilation output, test results, build logs, or script output. Must prove execution. "It should work" and placeholder assertions are rejected, (5) expose REMAINING GAPS — outstanding tasks, out-of-scope items, assumptions, manual checks. "No gaps" without explicit audit means you have not looked, (6) commit to your VERDICT — if the pivots say incomplete, the verdict must say incomplete. If rejected, fix the highlighted issue before declaring the task finished.

Structured reflection tool to verify task completion and delivery integrity. Forces the agent to prove it is actually finished — not "I think I am done" but mapping every user requirement to a specific file change, supplying execution logs as evidence, and identifying remaining gaps. Catches Incomplete Requirements (declaring done when 3 of 5 requirements are addressed), Unmodified Artifacts (claiming changes without specifying which files at which lines), Unverified Changes (no compilation logs, no test output, no build results — "it should work"), Gap Blindness (assuming 100% completion without listing outstanding work or limitations), and Delivery Flaws (placeholders, TODOs, or stub implementations left in committed code). Call at the end of every task execution
- **validate_critical_thinking**: The goal is not to reach "the right answer" — it is to reach a DEFENSIBLE answer with explicit assumptions, competing perspectives, balanced evidence, mapped consequences, and bounded confidence. You must: (1) surface HIDDEN ASSUMPTIONS — every problem has embedded assumptions about causality, scope, stakeholders, definitions, and constraints. "No assumptions" means you have not looked. Challenge each: what if this assumption is wrong? What depends on it?, (2) apply MULTIPLE COMPETING FRAMEWORKS — not "different angles" but NAMED mental models. First-principles vs analogical, economic vs behavioral, short-term vs long-term, stakeholder A vs stakeholder B. If two frameworks agree, you have not found a real alternative, (3) weigh evidence FOR AND AGAINST with EQUAL rigor — structure as FOR [data], AGAINST [data], NET [balanced assessment]. If you only have supporting evidence, you have confirmed, not searched. Actively seek the strongest counterargument — steelman the opposition, (4) trace SECOND-ORDER EFFECTS — who loses when this succeeds? What feedback loops does it create? What unintended incentives emerge? What resources does it consume? Every action has ripple effects — map at least 3, (5) BOUND your confidence — what specific evidence would change your conclusion? Under what conditions does it hold? What would weaken it? What would reverse it? "100% certain" means you have stopped thinking. "It depends" means you have not started. State a confidence level with conditions. If rejected, your reasoning has a structural blind spot.

Structured reflection tool for critical thinking on complex problems. Forces the agent to reason deeply BEFORE committing to a conclusion — surfacing hidden assumptions, applying multiple competing frameworks, weighing evidence for AND against, tracing second-order consequences, and bounding confidence with falsification conditions. Catches Assumption Blindness (taking embedded assumptions as facts — "users want speed" when the real bottleneck is trust), Mono-Perspective Reasoning (analyzing from one framework only — "economically optimal" while ignoring behavioral, political, and ethical dimensions), Confirmation Bias (only finding evidence FOR the conclusion — if you have zero counterexamples, you have not searched, you have confirmed), Scope Neglect (ignoring second-order effects — "this optimizes X" without asking who loses, what feedback loops emerge, what incentives change), and False Precision ("100% certain" or "it depends" — both are intellectual abdication. One refuses to think, the other refuses to commit). Call once per complex problem or decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Critical Thinking Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should we migrate our monolith to microservices? Our deployment frequency is low and the codebase is getting hard to maintain."

**🤖 AI Agent:**
> Verdict: ASSUMPTION_BLIND. Hidden assumptions unexamined. (1) You assume the monolith IS the cause of low deploy frequency — what if it's CI/CD, test coverage, or approval processes? (2) You assume 'hard to maintain' means 'needs decomposition' — what if it means 'needs better module boundaries within the monolith'? (3) You assume your team CAN operate a distributed system — microservices trade deployment complexity for operational complexity. Surface these assumptions first.

---

**👤 You:**
> "Assumptions validated: 70% of PRs touch 3+ modules (coupling confirmed). Team has 2 distributed-systems engineers, no K8s. Migration 6-12mo minimum. Frameworks: Conway's Law (3 teams → 3 services), cost-of-delay (coupling compounds quarterly). FOR: Shopify modular monolith cut deploy time 40%. AGAINST: Segment failed, re-monolithed. Second-order: training cost, velocity drop, on-call expansion. Confidence: 65% modular monolith correct. Would reverse with K8s or coupling <30%."

**🤖 AI Agent:**
> Verdict: REASONING_PROVEN. Assumptions exposed and validated with data (70% cross-module PRs). Multiple frameworks applied (Conway's Law, cost-of-delay). Evidence weighed impartially (Shopify FOR, Segment AGAINST). Consequences traced (training, velocity drop, on-call). Confidence bounded (65%, with reversal conditions). Conclusion is substantive: modular monolith over full microservices, given team constraints. This reasoning withstands scrutiny.

---

**👤 You:**
> "AI will replace 80% of software engineering jobs within 5 years. The evidence clearly shows this is inevitable. There are no counterarguments."

**🤖 AI Agent:**
> Verdict: CONFIRMATION_BIASED. Triple failure. (1) 'The evidence clearly shows' — which evidence? Every tech revolution prediction (paperless office, end of programming) has been wrong on timeline. Where is CONTRADICTING evidence? (2) 'No counterarguments' is a red flag — Jevons Paradox shows automation historically INCREASES total employment by lowering costs and expanding demand. (3) '80% within 5 years' is false precision. What would need to be true? What would falsify it?

---

**👤 You:**
> "I'm finished with the code migration. The build completes with no errors. No additional changes needed."

**🤖 AI Agent:**
> Verdict: UNVERIFIED_CHANGES. Contradiction: files modified but changes are not verified, yet the verdict is "DELIVERY_PROVEN". Run testing commands or build tasks to prove correctness. Assuming code works without executing it leads to broken pipelines. Please provide actual execution outputs in the verificationLogs field.


## ❓ FAQ

**Q: Does Critical Thinking Prover generate answers to complex problems?**
No. Critical Thinking Prover performs zero content generation. It forces the AI agent to structure its own reasoning into verifiable fields — assumptions, frameworks, evidence, consequences, confidence bounds — then validates that the reasoning is logically consistent. The agent does all the thinking. The tool catches blind spots.

**Q: How is this different from Sequential Thinking?**
Sequential Thinking structures thoughts in a linear chain — step 1, step 2, step 3. It's domain-agnostic and doesn't validate reasoning quality. Critical Thinking Prover is orthogonal: it doesn't sequence thoughts, it validates that the reasoning addresses five specific cognitive failure modes — assumption blindness, mono-perspective, confirmation bias, scope neglect, and false precision. You can use both together: Sequential Thinking to decompose the problem, Critical Thinking Prover to validate the conclusion.

**Q: What types of problems does this apply to?**
Any complex problem where the answer is not obvious and the reasoning matters more than the conclusion. Technical architecture decisions, business strategy, policy design, ethical dilemmas, resource allocation, organizational restructuring, risk assessment, investment analysis, product prioritization. If the problem has competing frameworks, hidden trade-offs, and uncertain outcomes — this tool forces the agent to reason through them instead of pattern-matching to a confident-sounding answer.

**Q: Can the agent still reach a 'wrong' conclusion after passing validation?**
Yes — and that's by design. Critical Thinking Prover validates reasoning PROCESS, not reasoning OUTCOMES. A conclusion can be well-reasoned and still turn out wrong — that's the nature of complex problems. What the tool guarantees is that the reasoning considered assumptions, multiple perspectives, counterevidence, consequences, and uncertainty bounds. A well-structured wrong answer is infinitely more useful than a confidently stated right one — because you can see WHERE the reasoning might break.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/critical-thinking-prover](https://vinkius.com/mcp/critical-thinking-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Critical Thinking Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `critical-thinking-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Critical Thinking Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "critical-thinking-prover": {
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

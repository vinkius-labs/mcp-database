# Delivery Integrity Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/delivery-integrity-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forces AI agents to reflect on task execution, matching prompt requirements to actual changes, verifying logs, and declaring gaps before claiming completion.

## Description
Claiming a task is complete when code contains placeholders, lacks test validation, or ignores minor requirements is a common failure mode in AI-driven development. Delivery Integrity Prover acts as a quality gate, forcing agents to map user prompt requirements to target files, verify actual execution logs, and trace outstanding work before declaring a task finished.

### The Problem It Solves

AI agents routinely rush to output a "task complete" message due to four cognitive flaws:

- **False completion claims** — Declaring success without verifying that all code chunks were written or that target files actually exist.
- **Unverified assumptions** — Assuming code compiles or tests pass without running verification scripts.
- **Gap blindness** — Overlooking edge cases, missing file migrations, or failing to declare remaining tasks that need human validation.
- **Placeholder neglect** — Leaving TODO comments or half-finished helper functions in the code base.

### How It Works

Delivery Integrity Prover validates completion status against 5 critical Decision Pivots:

1. **requirementsMapped** — Has every requirement from the user prompt been traced to specific file changes or actions?
2. **artifactsModified** — Have all target files been updated with zero placeholders or incomplete functions?
3. **verificationExecuted** — Have builds, compile scripts, or test suites been run with their logs supplied?
4. **gapsIdentified** — Have remaining tasks, out-of-scope items, or manual review requirements been defined?
5. **integrityProven** — Is the overall implementation verified, clean, and complete?

### Why It Works

- **Cognitive friction.** Adding structured checks breaks the LLM bias towards premature task closure, forcing the agent to self-correct before presenting the output.
- **Empirical evidence.** Demanding command execution outputs and logs stops the agent from guessing that code compiles.


## Available Tools (1)
- **verify_delivery**: "I think I am done" is not proof — only evidence is proof. You must: (1) state the OBJECTIVE — what was the user's actual request? Quote, do not interpret, (2) CHECKLIST every requirement — each requirement from the prompt mapped to a specific file change or action taken. "Addressed all requirements" is not a checklist. If the user asked for 5 things, show 5 mappings, (3) list MODIFIED FILES — exact paths with line ranges. "Updated the code" is not traceability. "src/auth.ts:L47-52 — fixed token refresh logic" is traceability, (4) provide VERIFICATION LOGS — compilation output, test results, build logs, or script output. Must prove execution happened. "It should work" and placeholder assertions are rejected, (5) expose REMAINING GAPS — outstanding tasks, out-of-scope items, assumptions, manual checks. "No gaps" without explicit audit means you have not looked. Every delivery has something left, (6) commit to your VERDICT — if the pivots say incomplete, the verdict must say incomplete. Optimistic verdicts with failing pivots are rejected. If rejected, fix the highlighted issue before declaring the task finished.

Structured validation tool to prove delivery integrity at task completion. Forces the agent to MAP every user requirement to a specific file change, SUPPLY execution logs as evidence, and EXPOSE remaining gaps — not "I think I am done" but provable completion. Catches Incomplete Requirements (declaring done when 3 of 5 requirements are addressed — the agent satisfies the "spirit" of the request while missing explicit sub-tasks), Unmodified Artifacts (claiming changes without specifying which files at which lines — "updated the code" is not traceability), Unverified Changes (no compilation logs, no test output, no build results — "it should work" is not evidence. If you did not run it, you did not verify it), Gap Blindness (assuming 100% completion without listing outstanding work, assumptions, or manual verification steps — "no gaps" without explicit audit means you have not looked), and Delivery Flaws (placeholders, TODOs, stub implementations, or commented-out code left in committed files — incomplete code presented as complete). Call at the end of EVERY task execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delivery Integrity Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have successfully finished creating the user profiles page. I edited the view files."

**🤖 AI Agent:**
> Verdict: INCOMPLETE_REQUIREMENTS. You claimed completion but did not map the prompt instructions to specific changes. Document how every requirement was implemented and check your pivots.

---

**👤 You:**
> "Task: Create page speed middleware. Checklist: SpeedMiddleware parses headers (verified in src/middleware.ts:L12-30). Files: src/middleware.ts. Logs: npm run test output shows '12 tests passed, 0 failed' after running MiddlewareSuite. Gaps: Bypassed checking on dynamic routes, needs manual verification on live server. Pivots: all true. Verdict: DELIVERY_PROVEN."

**🤖 AI Agent:**
> Verdict: DELIVERY_PROVEN. Requirements are mapped, middleware files updated, test logs provided, and route parsing limitations documented. Delivery verified.

---

**👤 You:**
> "Task: Create page speed middleware. Checklist: SpeedMiddleware parses headers. Files: src/middleware.ts. Logs: Everything worked fine when compiling. Gaps: none. Pivots: requirementsMapped=true, artifactsModified=true, verificationExecuted=true, gapsIdentified=true, integrityProven=true. Verdict: DELIVERY_PROVEN."

**🤖 AI Agent:**
> Verdict: UNVERIFIED_CHANGES. Your verification logs are a placeholder ('Everything worked fine'). Execute actual test or compile commands and provide the real console output to verify integrity.


## ❓ FAQ

**Q: Why are placeholder logs like 'tests passed' rejected?**
AI agents frequently assume that code works without executing it. Requiring actual command output logs forces them to run verification scripts, catching syntax errors and test failures early.

**Q: What counts as a remaining gap?**
A remaining gap includes any manual check required by the user, edge cases that were explicitly left out of scope, or dependencies on other teams. Banning 'none' forces agents to acknowledge limitations.

**Q: How does this prevent agents from lying about completion?**
It converts simple guidelines into strict tool-call checks. The agent must successfully match requirements to modified code lines and paste actual command outputs to get an approval verdict.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delivery-integrity-prover](https://vinkius.com/mcp/delivery-integrity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delivery Integrity Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `delivery-integrity-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delivery Integrity Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delivery-integrity-prover": {
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

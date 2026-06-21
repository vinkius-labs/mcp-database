# Delivery Integrity Prover MCP Server

Forces AI agents to reflect on task execution, matching prompt requirements to actual changes, verifying logs, and declaring gaps before claiming completion.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/delivery-integrity-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Available Tools
- **verify_delivery**: "I think I am done" is not proof — only evidence is proof. You must: (1) state the OBJECTIVE — what was the user's actual request? Quote, do not interpret, (2) CHECKLIST every requirement — each requirement from the prompt mapped to a specific file change or action taken. "Addressed all requirements" is not a checklist. If the user asked for 5 things, show 5 mappings, (3) list MODIFIED FILES — exact paths with line ranges. "Updated the code" is not traceability. "src/auth.ts:L47-52 — fixed token refresh logic" is traceability, (4) provide VERIFICATION LOGS — compilation output, test results, build logs, or script output. Must prove execution happened. "It should work" and placeholder assertions are rejected, (5) expose REMAINING GAPS — outstanding tasks, out-of-scope items, assumptions, manual checks. "No gaps" without explicit audit means you have not looked. Every delivery has something left, (6) commit to your VERDICT — if the pivots say incomplete, the verdict must say incomplete. Optimistic verdicts with failing pivots are rejected. If rejected, fix the highlighted issue before declaring the task finished.

Structured validation tool to prove delivery integrity at task completion. Forces the agent to MAP every user requirement to a specific file change, SUPPLY execution logs as evidence, and EXPOSE remaining gaps — not "I think I am done" but provable completion. Catches Incomplete Requirements (declaring done when 3 of 5 requirements are addressed — the agent satisfies the "spirit" of the request while missing explicit sub-tasks), Unmodified Artifacts (claiming changes without specifying which files at which lines — "updated the code" is not traceability), Unverified Changes (no compilation logs, no test output, no build results — "it should work" is not evidence. If you did not run it, you did not verify it), Gap Blindness (assuming 100% completion without listing outstanding work, assumptions, or manual verification steps — "no gaps" without explicit audit means you have not looked), and Delivery Flaws (placeholders, TODOs, stub implementations, or commented-out code left in committed files — incomplete code presented as complete). Call at the end of EVERY task execution


## Installation & Usage

To install and use the **Delivery Integrity Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delivery-integrity-prover](https://vinkius.com/mcp/delivery-integrity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Critical Thinking Prover MCP Server

AI agents accept premises without questioning, analyze from one perspective, cherry-pick evidence, ignore consequences, and present uncertainty as certainty. This tool forces rigor: surface assumptions, apply competing frameworks, weigh counterevidence, trace ripple effects, bound confidence.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/critical-thinking-prover)

## Overview
**Category:** productivity
**Tools Count:** 2

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


## Installation & Usage

To install and use the **Critical Thinking Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/critical-thinking-prover](https://vinkius.com/mcp/critical-thinking-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

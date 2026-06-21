# Context Integrity Prover MCP Server

AI forgets the original goal and hallucinates scope. This engine is a 6-pivot trap that forces the LLM to prove it hasn't drifted from the user's explicit constraints.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/context-integrity-prover)

## Overview
**Category:** reasoning
**Tools Count:** 1

## Description
LLMs suffer from context drift. You ask for a button, and 10 prompts later they are refactoring your database. The Context Integrity Prover is a cognitive trap designed to kill scope creep.

### The Semantic Trap

Before executing a plan, the agent must pass a strict 6-pivot validation:

1. **originalConstraintsMapped** — Re-state the exact constraints given at prompt 1.
2. **scopeBoundariesMaintained** — Define exactly what is NOT being built.
3. **outOfScopeRejected** — Explicitly reject a tangential idea.
4. **contextDriftPrevented** — Prove the current step aligns with the original goal.
5. **assumptionsValidated** — Ensure no hallucinated constraints were added.
6. **solutionMatchesOriginalIntent** — Final parity check.


## Available Tools
- **validate_context_integrity**: The most dangerous failure mode in multi-step reasoning is not being wrong — it is being right about the wrong problem. Each step may look reasonable, but cumulative drift can take you miles from the original request. You must: (1) MAP ORIGINAL CONSTRAINTS — quote the user's exact words. What did they ask for? What did they NOT ask for? What boundaries did they set? What is the precise deliverable? Do not paraphrase — quote. Paraphrasing introduces interpretation drift, (2) MAINTAIN SCOPE BOUNDARIES — define what you are NOT doing. Every task has a boundary. If you cannot name what is out of scope, you have not defined scope. List 3+ things that are explicitly out of scope for this task, (3) REJECT OUT OF SCOPE — explicitly identify and reject at least one tangential task that could be mistaken as in-scope. "While we are at it" and "it would also be nice to" are scope creep. Name the tangential task and state WHY it is out of scope, (4) PREVENT CONTEXT DRIFT — compare your current direction with the original request. Are you still solving the same problem? Has the solution evolved beyond what was asked? Check each step: does it serve the original intent, or has it become self-referential? (5) VALIDATE ASSUMPTIONS — list every assumption you are making that the user did NOT explicitly state. For each: is this assumption necessary? Did you invent a constraint? Could you ask instead of assuming? Hallucinated constraints are invisible — you believe them because you created them, (6) MATCH SOLUTION TO INTENT — prove the solution you are building matches the problem the user stated. Not the problem you find interesting. Not the problem you know how to solve. The problem they asked about. If rejected, you have drifted from the original intent. Re-read the user's request and start from their words.

Structured reflection tool for context integrity validation during multi-step execution. Forces the agent to prove the original user intent is preserved across every step — no scope creep, no context drift, no hallucinated constraints, no gold-plating. Catches Constraint Neglect (losing the original requirements mid-execution — the user said X, you are now doing Y), Scope Creep (adding unrequested features or analyses — "while we are at it" is the death of focus), Failure to Reject (accepting tangential tasks instead of explicitly declining out-of-scope work), Context Drift (progressive deviation from the original goal — each step looks reasonable but the cumulative direction is wrong), Hallucinated Constraints (inventing restrictions the user never stated — "we cannot do X" when nobody said that), and Intent Mismatch (the solution addresses a problem the user did not have). Call once before executing a multi-step plan, and again when you suspect drift


## Installation & Usage

To install and use the **Context Integrity Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context-integrity-prover](https://vinkius.com/mcp/context-integrity-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

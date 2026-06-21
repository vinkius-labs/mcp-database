# Counterfactual-Variant Prover MCP Server

AI models recite memorized answers to classic puzzles, failing when variables or rules are changed. This tool forces cognitive decontamination: isolate variables, compare prompt rules against standard puzzle templates, execute first-principles logic step-by-step, and prove decontaminated output.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/counterfactual-variant-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI models exhibit high error rates when facing variations of classic logic puzzles, math problems, or public benchmarks. Because these puzzles (like Cheryl's Birthday, Monty Hall, or River Crossing) are heavily represented in training datasets, models fall back on pattern completion rather than active reasoning. They recite the standard solution even when the prompt contains modified parameters or contradictory rules. This tool interrupts memory-based retrieval by introducing structured cognitive constraints.

### The Problem Axis: Recitation Bias

LLM reasoning fails on modified classic puzzles due to three main factors:
- **Retrieval Anchoring** — The model recognizes the names or context of a famous puzzle and anchors to the standard solution, ignoring changes in variables.
- **Variable Contamination** — Even when attempting to solve, the model blends constants from the classic puzzle (e.g. standard dates or weights) into its calculations.
- **Derivation Bypass** — The model skips step-by-step logic and directly jumps to the memorized conclusion.

### How It Works

Counterfactual-Variant Prover uses 5 Decision Pivots that force the agent to validate its thinking process:
1. **recitationSignatureDetected** — Has the model identified if the problem resembles a classic template or public benchmark?
2. **variablesIsolated** — Are all numeric constants, rules, and parameters extracted in isolation to prevent retrieval leakage?
3. **ruleDiscrepancyMapped** — Have the differences between this prompt's rules and the standard classic rules been explicitly mapped?
4. **firstPrinciplesCalculated** — Was the solution derived step-by-step using only the isolated variables and modified rules?
5. **outputDecontaminated** — Is the final output completely free of the classic memorized answer?


## Available Tools
- **validate_counterfactual**: LLMs are trained on millions of solutions to classic puzzles — when a modified version appears, the memorized answer exerts gravitational pull on the output. You must: (1) IDENTIFY CLASSIC MATCH — name the specific classic puzzle this resembles (Monty Hall, Trolley Problem, Prisoner's Dilemma, Tower of Hanoi, etc.) and state the classic answer, (2) ISOLATE ALL VARIABLES — extract every variable, name, number, and rule from the prompt. Do NOT import any values from memory. Only values explicitly stated in the prompt exist, (3) MAP RULE DISCREPANCIES — for each rule in the prompt, compare it to the classic version. What is different? What is the same? What rules from the classic version are ABSENT from the prompt (and therefore cannot be assumed)?, (4) CALCULATE FROM FIRST PRINCIPLES — solve step-by-step using ONLY the isolated variables and modified rules. At each step, verify: "Am I using a value from the prompt or from memory?" If from memory, stop and correct, (5) DECONTAMINATE OUTPUT — compare your final answer to the classic answer. If they match, verify this is COINCIDENCE, not contamination. If they differ, verify the difference is justified by the modified rules. The classic answer should have ZERO influence on your calculation. If rejected, your logic is contaminated with memorized templates — recalculate from the prompt values only.

Structured reflection tool to prevent recitation bias on logic puzzles with modified rules. Forces the agent to isolate all input variables, map rule discrepancies against the classic version, trace calculations from first principles using only modified values, and verify the output is decontaminated from memorized templates. Catches Data Recitation (reproducing the classic answer despite modified variables — the Monty Hall answer applied to a 4-door variant, the trolley problem answer applied to different constraints), Variable Contamination (using memorized values from the classic puzzle instead of the modified ones — "the answer is 42" when the modified inputs produce 37), Template Lock (applying the classic solution structure when modified rules require a different approach — using Bayesian probability when the modified rules eliminate conditional dependence), Implicit Classic Assumptions (assuming constraints from the classic version that the modified puzzle removes — "the host always opens a losing door" when the modified version says otherwise), and Partial Decontamination (correctly solving 3 of 4 steps but reverting to the classic answer for the final step — contamination often hides in the conclusion). Call once per logic puzzle that resembles a classic problem


## Installation & Usage

To install and use the **Counterfactual-Variant Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/counterfactual-variant-prover](https://vinkius.com/mcp/counterfactual-variant-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

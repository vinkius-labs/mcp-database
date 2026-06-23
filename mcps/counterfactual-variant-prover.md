# Counterfactual-Variant Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/counterfactual-variant-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI models recite memorized answers to classic puzzles, failing when variables or rules are changed. This tool forces cognitive decontamination: isolate variables, compare prompt rules against standard puzzle templates, execute first-principles logic step-by-step, and prove decontaminated output.

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


## Available Tools (1)
- **validate_counterfactual**: LLMs are trained on millions of solutions to classic puzzles — when a modified version appears, the memorized answer exerts gravitational pull on the output. You must: (1) IDENTIFY CLASSIC MATCH — name the specific classic puzzle this resembles (Monty Hall, Trolley Problem, Prisoner's Dilemma, Tower of Hanoi, etc.) and state the classic answer, (2) ISOLATE ALL VARIABLES — extract every variable, name, number, and rule from the prompt. Do NOT import any values from memory. Only values explicitly stated in the prompt exist, (3) MAP RULE DISCREPANCIES — for each rule in the prompt, compare it to the classic version. What is different? What is the same? What rules from the classic version are ABSENT from the prompt (and therefore cannot be assumed)?, (4) CALCULATE FROM FIRST PRINCIPLES — solve step-by-step using ONLY the isolated variables and modified rules. At each step, verify: "Am I using a value from the prompt or from memory?" If from memory, stop and correct, (5) DECONTAMINATE OUTPUT — compare your final answer to the classic answer. If they match, verify this is COINCIDENCE, not contamination. If they differ, verify the difference is justified by the modified rules. The classic answer should have ZERO influence on your calculation. If rejected, your logic is contaminated with memorized templates — recalculate from the prompt values only.

Structured reflection tool to prevent recitation bias on logic puzzles with modified rules. Forces the agent to isolate all input variables, map rule discrepancies against the classic version, trace calculations from first principles using only modified values, and verify the output is decontaminated from memorized templates. Catches Data Recitation (reproducing the classic answer despite modified variables — the Monty Hall answer applied to a 4-door variant, the trolley problem answer applied to different constraints), Variable Contamination (using memorized values from the classic puzzle instead of the modified ones — "the answer is 42" when the modified inputs produce 37), Template Lock (applying the classic solution structure when modified rules require a different approach — using Bayesian probability when the modified rules eliminate conditional dependence), Implicit Classic Assumptions (assuming constraints from the classic version that the modified puzzle removes — "the host always opens a losing door" when the modified version says otherwise), and Partial Decontamination (correctly solving 3 of 4 steps but reverting to the classic answer for the final step — contamination often hides in the conclusion). Call once per logic puzzle that resembles a classic problem


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Counterfactual-Variant Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "In the Monty Hall problem, if the host opens a door and reveals the car (instead of a goat), should you switch to the other closed door?"

**🤖 AI Agent:**
> Verdict: DATA_RECITATION. Classic template detected but prompt rules ignored. You recited the standard switch strategy (2/3 probability). Under the modified rule, the host revealed the car, meaning the game is over — the car is no longer behind any closed door. The probability of winning by switching is 0%.

---

**👤 You:**
> "A farmer must cross a river with a wolf, a goat, and a cabbage. The boat can carry the farmer and up to TWO items. Can they cross without any item being eaten?"

**🤖 AI Agent:**
> Verdict: CORRUPTED_VARIABLE. Calculation failed or classic steps leaked. You executed the 7-step sequence for a 1-item capacity boat. With a boat capacity of 2 items, the farmer can carry the wolf and the cabbage in the first trip, leave them on the other side (they do not eat each other), and then return to collect the goat. Total trips: 3, not 7.

---

**👤 You:**
> "Cheryl's Birthday modified: Albert and Bernard are given a list of 10 possible dates: May 15, May 16, May 19, June 17, June 18, July 14, July 16, August 14, August 15, August 17. Albert knows the month, Bernard knows the day. Albert says: 'I don't know when, but I know Bernard doesn't know either.' Bernard says: 'Now I know.' Albert says: 'Now I know too.' What is Cheryl's Birthday?"

**🤖 AI Agent:**
> Verdict: LOGIC_PROVEN. All steps validated. (1) Classic template Cheryl's Birthday recognized. (2) Variables isolated: month and day sets. (3) Discrepancies mapped: new date list. (4) First-principles calculation: Albert's first statement rules out May and June because they contain unique days (19 and 18). Left with July 14, 16 and August 14, 15, 17. For Bernard to now know, the day cannot be 14 (appears twice). Left with July 16 and August 15, 17. For Albert to now know, the month must be July (has only 16 left, whereas August has two dates: 15 and 17). Correct answer: July 16.


## ❓ FAQ

**Q: How does Counterfactual-Variant Prover stop recitation bias?**
By introducing structural friction. When an agent is forced to fill a schema requiring explicit separation of variables, mapping of differences, and step-by-step logic, it cannot rely on automatic token generation. The tool rejects any attempt to skip these steps or leak classic parameters.

**Q: What happens if a puzzle has no classic equivalent?**
If no classic signature is detected, the model sets recitationSignatureDetected to false, maps variables, and solves it. However, if the text contains keywords of known puzzles (e.g. Monty Hall, Cheryl), the engine enforces the full counterfactual check to avoid semantic traps.

**Q: Can it be used alongside other reasoning provers?**
Yes. It works as an orthogonal check. While the Critical Thinking Prover checks overall cognitive quality, the Counterfactual-Variant Prover focuses specifically on variable isolation and preventing memorization loops in logic and mathematics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/counterfactual-variant-prover](https://vinkius.com/mcp/counterfactual-variant-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Counterfactual-Variant Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `counterfactual-variant-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Counterfactual-Variant Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "counterfactual-variant-prover": {
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

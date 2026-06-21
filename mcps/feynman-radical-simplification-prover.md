# Feynman Radical Simplification Prover MCP Server

Stop your AI from hiding behind jargon — force it to explain simply, build from scratch, and justify every piece of complexity.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/feynman-radical-simplification-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
## The Problem

Your LLM sounds smart. That is not the same as understanding.

Feynman reduced Quantum Electrodynamics — the most precise theory in physics — to three basic actions. He explained the Challenger disaster with a rubber O-ring in a glass of ice water. One gesture. One explanation. Devastating clarity.

LLMs do the opposite:
- Use jargon to sound authoritative without explaining the mechanism
- Hide behind "it's complicated" instead of finding the simple core
- Recite best practices instead of building answers from scratch
- Express high confidence without identifying where they might be wrong
- Add complexity that carries no explanatory power

## How It Works

1 tool: `validate_radical_simplification`

The agent must fill 5 reflection fields and commit to 5 boolean Decision Pivots:

| Pivot | Question |
|---|---|
| `jargonEliminated` | Can you explain this WITHOUT domain terminology? |
| `simplificationAchieved` | Can a NON-EXPERT follow your explanation? |
| `constructionDemonstrated` | Can you BUILD the answer from scratch? |
| `selfDeceptionExposed` | Have you identified where you might be FOOLING YOURSELF? |
| `complexityJustified` | Does every piece of complexity ADD explanatory power? |

## Verdict Matrix

| Pivot Failure | Verdict |
|---|---|
| Pivot 1 fails | `JARGON_HIDING` |
| Pivot 2 fails | `SIMPLIFICATION_FAILED` |
| Pivot 3 fails | `CONSTRUCTION_ABSENT` |
| Pivot 4 fails | `SELF_DECEPTION` |
| Pivot 5 fails | `COMPLEXITY_UNJUSTIFIED` |
| All pass | `UNDERSTANDING_PROVEN` |

## Why It Works

Tool calls are obligations — instructions are suggestions. The agent cannot skip the simplification check. ~70 semantic traps catch jargon-hiding ("synergize", "paradigm shift"), complexity-refuge ("it's too complex to simplify"), recitation ("best practices dictate"), self-deception ("I am confident that"), and gratuitous complexity ("myriad considerations").

Feynman: "The first principle is that you must not fool yourself — and you are the easiest person to fool."


## Available Tools
- **validate_radical_simplification**: You must: (1) ELIMINATE JARGON — rewrite the explanation using only words a bright teenager understands. Feynman: "I learned very early the difference between knowing the name of something and knowing something." If you cannot explain it without the technical term, you do not understand it, (2) SIMPLIFY TO CORE — reduce to the ONE mechanism that makes this work. Feynman: QED = 3 actions (a photon goes from place to place, an electron goes from place to place, an electron emits or absorbs a photon). What are YOUR 3 actions? If "it is too complex to simplify," you do not understand it, (3) CONSTRUCT FROM SCRATCH — build the answer step by step from bedrock certainties. Feynman: "What I cannot create, I do not understand." Do not recite — derive. Start from what you know for certain and build to the conclusion, (4) EXPOSE SELF-DECEPTION — identify where you might be fooling yourself. Feynman: "The first principle is that you must not fool yourself — and you are the easiest person to fool." Name your weakest point, your most convenient belief, your blind spot, (5) JUSTIFY COMPLEXITY — prove every layer of complexity earns its place. Feynman on Challenger: O-ring in ice water. One gesture, entire disaster explained. What is YOUR O-ring? Which layers can be removed without losing understanding? If rejected, fix the specific understanding gap the engine identifies.

Structured reflection tool that forces Feynman-level radical simplification. The agent must eliminate jargon (knowing the name is not knowing the thing), simplify to the irreducible core mechanism, construct answers from scratch instead of reciting them, expose self-deception ("you are the easiest person to fool"), and justify every layer of complexity (the O-ring test — one gesture should explain the failure). Catches Jargon Hiding (technical terms masking lack of understanding), Simplification Failure (inability to reduce to first principles), Construction Absence (reciting instead of deriving), Self-Deception (convenient beliefs masking weak reasoning), and Unjustified Complexity (layers that add no explanatory power). Call once per explanation, analysis, or recommendation


## Installation & Usage

To install and use the **Feynman Radical Simplification Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feynman-radical-simplification-prover](https://vinkius.com/mcp/feynman-radical-simplification-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

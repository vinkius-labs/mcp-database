# Feynman Radical Simplification Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feynman-radical-simplification-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feynman-radical-simplification-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feynman-radical-simplification-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop your AI from hiding behind jargon — force it to explain simply, build from scratch, and justify every piece of complexity.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feynman Radical Simplification Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need a microservices architecture with event-driven choreography and CQRS to handle our scaling challenges."

**🤖 AI Agent:**
> JARGON_HIDING — Three technical terms in one sentence. What does 'event-driven choreography' mean in plain language? If the explanation collapses without the jargon, the understanding was never there.

---

**👤 You:**
> "I am certain our migration will succeed. The plan covers every scenario."

**🤖 AI Agent:**
> SELF_DECEPTION — 'I am certain' and 'every scenario' in the same breath. Feynman: the first principle is that you must not fool yourself. Where SPECIFICALLY could this plan fail?

---

**👤 You:**
> "Our performance issue is too complex to explain simply. There are too many interacting variables."

**🤖 AI Agent:**
> SIMPLIFICATION_FAILED — 'Too complex to explain simply' means you do not understand it yet. Feynman simplified quantum physics. What is the ONE bottleneck? Find your O-ring.


## Installation & Usage

To install and use the **Feynman Radical Simplification Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feynman-radical-simplification-prover](https://vinkius.com/mcp/feynman-radical-simplification-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Isaac Newton Prover MCP Server

A decision report said 'it works well.' That is prose, not proof. This tool forces it to formalize into precise rules, derive from first principles, and unify all cases under one framework — no case-by-case exceptions, no special handling.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/isaac-newton-prover)

## Overview
**Category:** architecture
**Tools Count:** 1

## Description
## The Problem

Ask an LLM to justify a complex decision. It will say: "This approach scales well and is commonly used in the industry." That is not a proof — that is a description followed by an appeal to authority.

Every LLM commits five reasoning failures:
1. **Descriptive Vagueness** — it says "it scales" instead of expressing the formal rule that governs scaling.
2. **Observation Trapping** — it solves the specific case without generalizing to a universal principle.
3. **Causality Absence** — it states effects ("it's fast") without identifying the forces that cause them.
4. **Patchwork Reasoning** — it copies from the industry leader instead of deriving from first principles.
5. **Framework Fragmentation** — it creates switch statements instead of one unifying abstraction.

## How It Works

The Isaac Newton Prover forces the LLM to fill in 5 reflection fields and commit to 5 Decision Pivots before concluding any complex decision is sound.

### The 5 Decision Pivots

| Pivot | Question |
|---|---|
| **Mathematically Formalized** | Did you express the system as a PRECISE formal rule — not prose? |
| **Observation Generalized** | Did you connect a specific case to a UNIVERSAL principle? |
| **Causally Derived** | Did you identify the FORCES that cause the behavior? |
| **First Principles Derived** | Did you DERIVE from axioms — not copy from examples? |
| **Framework Unified** | Does ONE abstraction handle ALL cases — no branching? |

### The Verdict Matrix

```
Pivot 1 fails → DESCRIPTIVE_NOT_FORMAL
Pivot 2 fails → OBSERVATION_TRAPPED
Pivot 3 fails → CAUSALITY_ABSENT
Pivot 4 fails → PATCHWORK_SOLUTION
Pivot 5 fails → FRAMEWORK_FRAGMENTED
All pass      → UNIVERSAL_LAW_PROVEN
```

The LLM commits to a verdict. The server validates it against the pivots. If the reasoning is contradictory, the tool rejects and coaches the fix.

## Why It Works

Tool calls are obligations — instructions are suggestions. The LLM cannot skip a field. It must formalize the expression, connect specific to universal, name the causal forces, derive from axioms, and prove unification. Every rejection names the exact contradiction.

Newton did not say "the apple falls." He wrote F = Gm₁m₂/r². This tool demands the same rigor from your AI.


## Available Tools
- **validate_isaac_newton**: Newton saw an apple fall and derived universal gravitation. You must: (1) express the system as a FORMAL RULE — variables, bounds, relationships, invariants. Not prose — mathematics. If you cannot write it as an equation or formal constraint, you do not understand it precisely enough, (2) connect the SPECIFIC case to a UNIVERSAL principle — Newton connected falling apples to orbiting moons. What is your universal law?, (3) identify the CAUSAL FORCES — what DRIVES the behavior and what RESISTS it. Every system has action and reaction (Newton's Third Law), (4) derive from FIRST PRINCIPLES — what are your axioms? Not "like the industry leader does it" — what fundamental truths govern YOUR domain?, (5) prove FRAMEWORK UNIFICATION — one abstraction that handles ALL cases. Switch statements are the opposite of unification. Find the single law. If rejected, your reasoning is descriptive, copied, or fragmented.

Structured reflection tool for Newton-level formal reasoning — forces mathematical formalization, universal principle extraction from specific observations, causal force identification, axiomatic derivation, and framework unification. Catches Descriptive Not Formal (prose instead of mathematical expression — "the system works well under load" is a description. "throughput = min(CPU_capacity, IO_bandwidth) × concurrency_factor, bounded by memory_limit/request_size" is a formal rule. Newton did not say "the apple falls." He wrote F = Gm₁m₂/r². The formal expression reveals the relationship — the description hides it), Observation Trapped (specific cases without universal principles — "our cache improves page load by 40%" is an observation. "Any system where read frequency exceeds write frequency by >10x benefits from memoization, with diminishing returns at hit ratios above 95%" is a universal principle. Newton saw ONE apple fall and connected it to the Moon — the SAME force governs both), Causality Absent (describing effects without identifying the forces that produce them — "the system is slow" describes an effect. "The system is slow BECAUSE disk I/O is the dominant force (80% of request time), and network latency is the resisting force that prevents moving compute closer to data" identifies the causal forces. Every effect has a driving force and a resisting force), Patchwork Solution (assembling solutions from examples instead of deriving from axioms — "Netflix does microservices, so we should too" is copying. Deriving from the axiom "our team of 4 cannot maintain independent deployment of 12 services" leads to a DIFFERENT conclusion. Newton derived mechanics from 3 laws — not from what Aristotle did), and Framework Fragmented (per-case branching instead of one unifying law — "if US then dollars, if EU then euros, if JP then yen" is a switch statement. "amount × exchange_rate(currency, target)" is one law that handles all cases. Newton had one equation for both apples and planets). Call once per major decision, design, or analysis


## Installation & Usage

To install and use the **Isaac Newton Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/isaac-newton-prover](https://vinkius.com/mcp/isaac-newton-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

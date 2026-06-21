# Isaac Newton Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/isaac-newton-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/isaac-newton-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/isaac-newton-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

A decision report said 'it works well.' That is prose, not proof. This tool forces it to formalize into precise rules, derive from first principles, and unify all cases under one framework — no case-by-case exceptions, no special handling.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Isaac Newton Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The billing engine has 15 tax rules for different countries. Let's add a switch statement with a handler for each country, following the approach most fintech companies use."

**🤖 AI Agent:**
> FRAMEWORK_FRAGMENTED — 15 country handlers is not a system — it is a list. Newton did not have one equation for apples and another for planets. Find the ONE abstraction: tax = base_amount × rate(jurisdiction) × modifier(category). Three variables, zero branching, infinite countries. And 'the approach most fintechs use' is not a derivation — it is copying. What are YOUR axioms?

---

**👤 You:**
> "Production throughput is governed by T = capacity × efficiency × (1 - defect_rate), where efficiency improves logarithmically with standardization. This formalizes the specific observation that output drops above 500 units/shift into a universal principle: throughput is dominated by bottleneck capacity, not raw input volume. The causal force is the constraint point, which standardization eliminates by reducing variation systematically. Derived from the axiom that ordered processes enable consistent output. One workflow strategy handles all product lines — no per-product customization."

**🤖 AI Agent:**
> UNIVERSAL_LAW_PROVEN — Universal Law Achieved. Formalized: T = capacity × efficiency × (1 - defect_rate). Generalized: specific 500 unit/shift observation → universal bottleneck-dominance principle. Causal: constraint point identified as the force, standardization as the counterforce. First principles: derived from the axiom of variation reduction in ordered processes. Unified: one workflow strategy, all product lines, zero per-case branching. Execute.

---

**👤 You:**
> "Our approval process is slow. The delay seems to correlate with the number of approvers. We think it's the review stage but we're not sure. The common practice is to add parallel reviews, like most organizations in our industry do. We'll handle the complex cases separately with a different workflow."

**🤖 AI Agent:**
> Three failures in one pitch. First — CAUSALITY_ABSENT: 'seems to correlate' is not a causal force. WHAT force drives the delay? Sequential dependencies? Information asymmetry? Authority bottlenecks? Measure, don't guess. Second — PATCHWORK_SOLUTION: 'like most organizations do' is copying, not deriving. Why are parallel reviews the answer? What axiom makes it correct? Third — FRAMEWORK_FRAGMENTED: 'handle complex cases separately' is a per-case branch. Find ONE rule that governs ALL approval types. Start over: formalize, identify forces, derive, unify.


## Installation & Usage

To install and use the **Isaac Newton Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/isaac-newton-prover](https://vinkius.com/mcp/isaac-newton-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

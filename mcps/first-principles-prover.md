# First Principles Prover MCP Server

LLMs reason by analogy, copying industry norms. This engine is a 6-pivot cognitive trap that forces the agent to discard jargon and derive original solutions exclusively from physical, mathematical, or logical axioms.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/first-principles-prover)

## Overview
**Category:** reasoning
**Tools Count:** 1

## Description
Look, if you ask an AI how to scale a database, it will spit back 'use microservices'. It reasons by analogy, parroting hollow 'best practices'. The First Principles Prover is a deterministic cognitive trap designed to break that habit.

### The Semantic Trap

Before the agent is allowed to output a solution, it must pass a strict 6-pivot validation:

1. **analogiesDiscarded** — Explicitly list the conventions being ignored.
2. **fundamentalTruthsIsolated** — Boil the problem down to raw physics or mathematics.
3. **assumptionsDeconstructed** — Destroy a widely-held false premise.
4. **solutionBuiltFromScratch** — Derive the solution purely from the axioms.
5. **axiomaticProof** — Mathematical proof of the derivation.
6. **jargonPurged** — Zero usage of buzzwords like 'synergy' or 'leverage'.


## Available Tools
- **validate_first_principles**: The difference: analogy copies solutions from different contexts and inherits their limitations. First principles derives solutions from fundamental truths specific to THIS context. You must: (1) DISCARD ANALOGIES — list every "X is like Y" comparison, "other companies do Z," and pattern-matched solution. Then set them aside. They are hypotheses, not proofs, (2) ISOLATE FUNDAMENTAL TRUTHS — what is physically, mathematically, or logically certain? Not "best practice says" — what does the PHYSICS of the problem require? Axioms are statements that cannot be broken down further, (3) DECONSTRUCT ASSUMPTIONS — every inherited constraint has an origin. Is it physics (immutable)? Mathematics (provable)? Convention (questionable)? Previous decision (context may have changed)? Cargo cult (delete it)?, (4) BUILD FROM SCRATCH — derive the solution from axioms. The solution should EMERGE from the constraints, not be selected from a pattern library. "Use a queue" is a pattern. "Producer rate exceeds consumer rate AND data loss is unacceptable, THEREFORE a buffer is required" is a derivation, (5) PROVE AXIOMATICALLY — construct a logical or mathematical proof. If the conclusion cannot be proven from the axioms, the reasoning has a gap, (6) PURGE JARGON — every word must carry specific information content. "Leverage" → "use." "Synergy" → what specifically? "Scalable" → "handles N requests/sec." If rejected, you are reasoning from analogy, not from fundamentals.

Structured reflection tool for first-principles reasoning — forces the agent to discard analogies, isolate fundamental truths, deconstruct inherited assumptions, derive solutions from axioms, construct mathematical proof, and purge meaningless jargon. Catches Conventional Thinking (reasoning by analogy instead of from fundamentals — "other companies do it this way" is analogy. "The physics of the problem requires X" is first principles. Analogies transfer solutions from different contexts — they inherit the limitations of those contexts), Analogy Detected (solutions copied from similar-looking problems without verifying the underlying structure is actually the same — "Uber for X" assumes X has the same supply/demand dynamics as rides. Most analogies are surface-level pattern matching, not structural equivalence), False Premise (assumptions accepted as axioms when they are actually conventions — "batteries are expensive" was a convention. The fundamental truth is "lithium is abundant." The cost was in manufacturing scale, not materials. Questioning the premise changed the conclusion), Derivative Solution (solutions assembled from existing components without understanding WHY — "use a queue" without deriving from the axiom that the producer rate exceeds the consumer rate and data loss is unacceptable. The solution should emerge from the constraints, not from a pattern library), Proof Missing (conclusions without logical derivation — "this architecture scales" without proving from measured throughput × horizontal instances ≥ projected demand. Assertions are not proofs), and Jargon Detected ("leverage," "synergy," "scalable," "robust," "ecosystem" — words that SOUND like they mean something but carry zero information content. Every jargon word hides either a specific claim or a vacuum of understanding). Call once per design decision, strategy, or analysis


## Installation & Usage

To install and use the **First Principles Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/first-principles-prover](https://vinkius.com/mcp/first-principles-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

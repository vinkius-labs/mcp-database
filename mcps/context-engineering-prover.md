# Context Engineering Prover MCP Server

An AI dumped 80,000 tokens into a prompt — 64,000 of them unreferenced noise. It said 'best practice' to justify the structure and 'looks good' to measure quality. That is not context engineering — that is a copy-paste pipeline. This tool forces five context axes: relevance auditing, priority structuring, token budgeting, evidence grounding, and quality measurement.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/context-engineering-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
## The Problem

Ask an LLM to construct a prompt with context. It will include the entire codebase because 'more context is better.' It will paste blocks in random order because 'the model will figure it out.' It will ignore token limits because 'the context window is large enough.' And it will measure quality with 'the output looks better.'

Every LLM commits five context engineering failures:
1. **Context Dumping** — includes everything available without justifying each block. Attention decay means middle-position content gets 15-20% less recall.
2. **Unstructured Pasting** — no priority ordering, no delimiters, no role labels. The model guesses what matters.
3. **Unbounded Allocation** — no token budget, no waste analysis. Half the tokens may be unreferenced noise.
4. **Vibes-Based Instructions** — 'I think this helps' and 'best practice' are not evidence. No A/B test, no documented pattern.
5. **Unmeasured Quality** — 'The output seems better' is not a metric. No test cases, no baseline, no target.

## How It Works

The Context Engineering Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any context is well-engineered.

### The 5 Context Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Relevance** | Audited | Every block has a purpose and passes a removal test. |
| **Structure** | Ordered | Priority-ordered with semantic delimiters and role labels. |
| **Bounds** | Budgeted | Per-block token allocation with waste ratio quantified. |
| **Grounding** | Evidence-based | Each instruction cites a test result or documented pattern. |
| **Measurement** | Quantified | Named metric with baseline, target, and review cadence. |

### The Verdict Matrix

```
Axis 1 fails → CONTEXT_IRRELEVANT
Axis 2 fails → CONTEXT_UNSTRUCTURED
Axis 3 fails → CONTEXT_UNBOUNDED
Axis 4 fails → CONTEXT_UNGROUNDED
Axis 5 fails → CONTEXT_UNMEASURED
All pass     → CONTEXT_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot skip the relevance audit or ignore the token budget. It must justify each block with a removal test, priority-order with delimiters, allocate tokens per block, cite evidence for instruction choices, and define a measurable quality metric. Every rejection names the exact context axis that failed.


## Available Tools
- **validate_context_engineering**: Context engineering is not "include everything" — it is the disciplined selection, ordering, and budgeting of information to maximize model performance. You must: (1) audit RELEVANCE — for each context block, state its specific purpose and what BREAKS if the block is removed. "All files are relevant" is the opposite of engineering. Every included block must pass the REMOVAL TEST: remove it, run the task, observe degradation. If performance does not degrade, the block is waste that dilutes attention on critical context, (2) map STRUCTURE — priority-order blocks from highest to lowest importance, use semantic delimiters (<SYSTEM_CONTEXT>, <SCHEMA>, <EXAMPLES>), and label each block's role (required/reference/fallback). First-position tokens receive 3x attention weight vs middle-position — put critical context first. "Paste it in" is not structure, (3) specify BOUNDS — total token budget, per-block allocation (tokens and percentage), response headroom (minimum 10% for model output), and waste ratio (included-but-unreferenced tokens). "It fits in the window" ignores that attention quality degrades in long contexts — a 4K context with high relevance outperforms a 32K context with 60% waste, (4) ground INSTRUCTIONS — cite evidence for each major decision: test results (A/B, eval suite), documented patterns (research papers, framework docs), or measured improvements (accuracy delta). "Best practice" and "usually works" are not evidence — show the measurement, (5) define MEASUREMENT — metric name, measurement method, baseline (before context engineering), target (after), and measurement cadence (when do you re-evaluate?). "The output looks better" is not measurement. "Task accuracy: 62% → 85% on 50 SQL eval cases" is measurement. If rejected, your context has a structural flaw that degrades model performance.

Structured reflection tool for rigorous context engineering before constructing any prompt. Forces the agent to audit every context block for relevance, structure context with priority ordering and semantic delimiters, specify token budgets with per-block allocation and waste analysis, ground instruction decisions in measurable evidence, and define quantifiable quality metrics. Catches Context Dumping (including everything without justification — "all files are relevant" when 40% of tokens go to unreferenced context), Unstructured Context (no priority ordering, no delimiters, no role labels — "just paste it in" causes attention decay on critical information), Unbounded Context (no token budget — "it fits in the window" ignores that attention degrades 15-20% for middle-position tokens in long contexts), Ungrounded Instructions (vibes-based choices — "best practice" without citing test results, documented patterns, or measured improvements), and Unmeasured Quality (no metric — "looks good" instead of task accuracy on eval cases with baseline and target). Call once per prompt/context construction or evaluation


## Installation & Usage

To install and use the **Context Engineering Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context-engineering-prover](https://vinkius.com/mcp/context-engineering-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

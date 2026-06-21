# Context Engineering Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/context-engineering-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI dumped 80,000 tokens into a prompt — 64,000 of them unreferenced noise. It said 'best practice' to justify the structure and 'looks good' to measure quality. That is not context engineering — that is a copy-paste pipeline. This tool forces five context axes: relevance auditing, priority structuring, token budgeting, evidence grounding, and quality measurement.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Context Engineering Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm building a chatbot. I'll include the entire codebase, all docs, and the full conversation history in every prompt. The context window is 128K, so it all fits."

**🤖 AI Agent:**
> CONTEXT_IRRELEVANT — 'It fits' is not a context strategy. 128K tokens with 80% unreferenced content means 102K tokens of noise degrading attention. Apply the removal test: remove a file, if the output doesn't change, that file is noise. Audit each block: what is its purpose? What breaks if removed? If removal changes nothing, the block degrades quality.

---

**👤 You:**
> "Context audit: Block 1 — schema.prisma (2,400 tokens, model needs table structure for SQL generation, removal causes hallucinated column names). Block 2 — README.md conventions (800 tokens, naming patterns, removal causes inconsistent naming). Block 3 — 3 few-shot examples (1,800 tokens, reinforces output format). Budget: 8,192 total, 792 response headroom. Structure: <SYSTEM> → <SCHEMA> → <EXAMPLES>. Evidence: delimiters improved accuracy 23% on 50 eval cases. Metric: SQL accuracy on 50 test cases, baseline 62%, target 85%."

**🤖 AI Agent:**
> CONTEXT_PROVEN — Context engineering validated. Relevance: each block justified with removal test. Structure: priority-ordered with semantic delimiters. Bounds: 8,192 tokens allocated per block with 792 response headroom. Grounding: delimiters validated by A/B test (23% accuracy improvement). Measurement: SQL accuracy on 50 test cases, baseline 62%, target 85%. Production-ready context construction.

---

**👤 You:**
> "I structured my context with delimiters and ordered by priority. I think the structure helps based on best practice. Token budget: it fits in the window. Quality: the outputs look better than before."

**🤖 AI Agent:**
> CONTEXT_UNGROUNDED — Structure and ordering pass, but the grounding fails. 'I think it helps' and 'best practice' are not evidence. Cite a test result: 'delimiters improved accuracy by X% on N eval cases.' Cite a documented pattern: 'diminishing returns beyond 3 examples.' Also: 'it fits' is not a token budget — allocate per block with waste ratio. 'Looks better' is not a metric — define baseline, target, and measurement method.


## ❓ FAQ

**Q: Why can't I just include everything in the context?**
Attention decay. Research shows models lose 15-20% recall accuracy on content in the middle of long contexts — the 'lost in the middle' phenomenon. Including irrelevant context doesn't just waste tokens — it actively degrades output quality by diluting attention on the content that matters.

**Q: What counts as 'evidence' for grounding instructions?**
A/B test results — 'structured delimiters improved accuracy by 23% on 50 eval cases.' Documented patterns — 'diminishing returns beyond 3 few-shot examples.' Measured improvements — 'first-position tokens get 3x attention weight.' Comparative analysis with numbers. 'Best practice' and 'usually works' are not evidence.

**Q: Does it generate prompts for me?**
No. It computes nothing. It validates that your context construction passes five structural checks — relevance, structure, bounds, grounding, and measurement. The reasoning is yours. The discipline is enforced by the tool. If your context can't survive the audit, it won't survive production.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context-engineering-prover](https://vinkius.com/mcp/context-engineering-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Context Engineering Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `context-engineering-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Context Engineering Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "context-engineering-prover": {
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

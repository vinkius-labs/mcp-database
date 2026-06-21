# Article Architect MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/article-architect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/article-architect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/article-architect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Technical blog posts written by AI read like documentation — step 1, step 2, step 3, no argument, no tradeoffs, no opinion. Article Architect forces the agent to take a position, expose limitations, plan code as evidence, cite production data, and define a reader transformation.

## Description
Ask an AI agent to write a technical blog post and you get the same thing every time: a tutorial disguised as an article. "Step 1: Install X. Step 2: Configure Y. Step 3: Deploy Z." No thesis, no tradeoffs, no opinion, no production experience, no reason for the reader to trust the author over the official documentation.

### The Problem It Solves

AI-generated technical articles fail on five axes:

- **No thesis** — describes WHAT something is without arguing WHY it matters or WHEN to use it. "Docker is a containerization platform" is Wikipedia, not a blog post.
- **One-sided** — presents every approach as universally good. No tradeoffs, no failure modes, no "when NOT to use this." Engineers distrust advocacy without honest limitations.
- **Decorative code** — code blocks that illustrate syntax but don't prove the argument. Hello-world examples the reader can find in the docs.
- **No production signal** — technically correct but clearly written by someone who never shipped it. No metrics, no failures, no surprises, no timelines.
- **Passive reader** — after reading, the reader "understands" the topic but can't DO anything new. No decision framework, no benchmark to run, no migration checklist.

These aren't writing problems. They're **thinking problems.** The agent never asks: what position am I taking? What does this cost? Can my code prove it? Have I seen this in production? What can the reader do after?

### How It Works

Article Architect uses 5 Decision Pivots that force the agent to architect the article's argumentative structure before writing a single paragraph:

1. **thesisStated** — Take a DEBATABLE position. Not "X is a framework" — "X reduced our deploy time by 73% but tripled debugging complexity."
2. **tradeoffsExposed** — When does this approach FAIL? What do you sacrifice? Real tradeoffs hurt: "You lose hot-reloading." "Debugging now spans 6 services."
3. **codeProves** — Every code block is EVIDENCE. Before/after comparisons, benchmarks, failing tests. If the reader can find it in the docs, cut it.
4. **experienceGrounded** — One concrete production detail: a metric, a failure, a surprise. Not "in production environments" — that's generic. "p95 dropped from 1.2s to 380ms after migrating 3 of 11 services."
5. **readerTransformed** — After reading, the reader can DO something: run a benchmark, apply a migration pattern, use a decision framework. Not "understand X."

The engine validates everything. If the thesis is a definition, it rejects. If tradeoffs are dismissive ("minor overhead"), it rejects. If code is boilerplate, it rejects. If experience uses generic phrases, it rejects. If the takeaway is "consider using X", it rejects.

### The Core Insight

The best technical blog posts are ARGUMENTS, not tutorials. Tutorials belong in documentation. A blog article takes a position that a smart engineer could disagree with, proves it with code and production data, honestly exposes the costs, and sends the reader away with a new capability. Article Architect enforces this standard.

### Language-Agnostic

Article Architect works for technical articles in any language. The pivots are universal: every language has theses, tradeoffs, code evidence, production grounding, and reader transformations.


## Available Tools
- **architect_article**: You must: (1) state a THESIS — a debatable position, NOT a description. "X is a framework" is Wikipedia. "X reduced our deploy time by 73% but tripled debugging complexity" is a thesis. (2) expose TRADEOFFS — when does this approach FAIL? What do you sacrifice? Engineers distrust one-sided advocacy. (3) plan CODE that PROVES the thesis — not hello-world, not boilerplate from the docs. Before/after comparisons, benchmarks, failing tests, performance traces. (4) ground it in PRODUCTION — at least one concrete detail: a metric, a failure, a surprise. "We hit X after 72 hours in production" transforms theory into authority. (5) define the TRANSFORMATION — after reading, what can the reader DO? Not "understand X" — an action: "run this benchmark", "apply this migration pattern", "use this decision framework". If the tool rejects, your article will read as AI-generated tutorial filler. Fix the architecture.

Structured reflection tool for architecting technical blog articles that argue, prove, and transform — not just describe. The agent must commit to a debatable thesis, expose honest tradeoffs, plan code blocks that serve as evidence, ground the argument in production experience, and define a concrete reader transformation. The tool validates logical consistency: if the thesis is a definition, it rejects. If tradeoffs are dismissive, it rejects. If code is boilerplate, it rejects. If experience is generic, it rejects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Article Architect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Write a technical blog post about React Server Components."

**🤖 AI Agent:**
> Verdict: NO_THESIS. 'About React Server Components' is a topic, not an argument. What POSITION are you taking? 'RSC eliminated 4 round trips from our checkout flow and cut payload by 62% — but it moved complexity to the resolver layer.' That's a thesis. Take a side. What did RSC fix, what did it break, and when should you NOT use it?

---

**👤 You:**
> "Thesis: tRPC cut type errors 89% and API surface 60%, but onboarding slowed 3x. Tradeoffs: steep learning curve, runtime overhead. Code: type-error diff, API surface comparison, onboarding metrics. Evidence: 14-service migration over 3 sprints."

**🤖 AI Agent:**
> Verdict: PUBLISH_READY. Thesis is debatable (speed vs onboarding cost). Tradeoffs are painful (3x onboarding). Code is evidence (type-error diffs, not hello-world). Production is concrete (14 services, 3 sprints). Architecture validated — write it.

---

**👤 You:**
> "Thesis: Kubernetes simplifies container orchestration. Tradeoffs: minor complexity overhead. Code: kubectl apply example. Evidence: widely used in production."

**🤖 AI Agent:**
> Multiple rejections. (1) NO_THESIS — 'simplifies container orchestration' is a marketing tagline, not a thesis. Compared to what? At what cost? (2) ONE_SIDED — 'minor complexity overhead' dismisses real pain. (3) ABSTRACT — kubectl apply is documentation, not evidence. (4) THEORETICAL — 'widely used in production' is generic. Fix all four.


## Installation & Usage

To install and use the **Article Architect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/article-architect](https://vinkius.com/mcp/article-architect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

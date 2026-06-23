# Editorial Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/editorial-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Every AI agent writes the same way — uniform sentences, identical rhythm, filler words. Editorial Prover breaks the pattern with a structured self-audit: name the reader, justify the hook, map the rhythm, find the weakest sentence, and prove the paragraph structure varies.

## Description
Every AI agent writes the same way. Uniform sentences, identical paragraph structures, filler words like "delve" and "leverage", hedging instead of committing, bullet lists instead of prose. Readers spot it instantly. Detectors flag it in seconds. Editorial Prover eliminates this problem at the source.

### The Problem It Solves

AI-generated text fails on five measurable axes — all documented in detection research (GPTZero 2024, Northeastern 2025, arXiv 2024):

- **Low burstiness** — every sentence is 15-20 words, same rhythm, like a metronome
- **Structural repetition** — paragraph 1 has the same shape as paragraph 2, 3, 4
- **Filler vocabulary** — "furthermore", "it's important to note", "in today's world"
- **Hedging** — "some believe", "it could be argued" — never commits to a position
- **Audience blindness** — writes for "everyone" which means no one

These aren't grammar problems. They're **thinking problems.** The agent never asks: who reads this? Does my opening grab? Which sentence should I cut?

### How It Works

Editorial Prover uses 5 Decision Pivots that force the writing agent to think through an editorial process. The tool computes nothing about the content — like Sequential Thinking, the act of answering structured questions IS the quality improvement.

For each section, the agent must:

1. **Name the reader** and what they desire (`readerDesire`)
2. **Justify the hook** — why does the opening grab? What position does it take? (`hookCommits`)
3. **Describe the rhythm** with specific word counts — "6-word opener, 28-word explanation, 4-word punch" (`rhythmConscious`)
4. **Identify the weakest sentence** and decide: keep, rewrite, or cut (`weakestIdentified`)
5. **Map paragraph structures** to prove variety — "P1: question→answer, P2: claim→evidence" (`structureVaries`)

The tool validates pivot consistency. If the agent claims varied rhythm but sentences are uniform (burstiness CV < 0.25), the tool rejects with measured proof.

### Why It Works

- **Thinking amplification, not detection.** The tool doesn't scan for bad words — it forces the agent to reason about its writing. The reasoning process IS the improvement.
- **Language-agnostic.** Works for any language — English, Portuguese, Japanese, Arabic. The pivots are universal editorial questions. The burstiness check is pure math on sentence lengths.
- **The commit pattern.** The agent must propose its own verdict (PUBLISH_READY, WEAK_HOOK, etc.) and the server validates consistency with the pivots. This forced commitment deepens the thinking.


## Available Tools (1)
- **audit_copy**: This is a self-audit — the act of answering these questions forces higher quality writing. Works for ANY language. You must: (1) name the SPECIFIC AUDIENCE — not "developers" but "backend engineers building CI/CD pipelines who are evaluating whether to build or buy their deployment tooling," (2) explain WHY your HOOK grabs — what position does the headline take? What promise does it make? What urgency does it create? A headline that merely describes the content is not a hook, (3) describe SENTENCE RHYTHM with word counts — vary consciously. Short punches (4-6 words) mixed with longer explanations (25-35 words). If all sentences are 15-20 words, the rhythm flatlines. Human writing has burstiness, (4) identify the WEAKEST SENTENCE — copy it, explain why it is weak, decide: keep, rewrite, or cut. Every section has a weakest sentence. Finding it makes the section stronger, (5) map PARAGRAPH STRUCTURES — each paragraph should have a different architecture. P1: question→answer. P2: claim→evidence. P3: story→lesson. P4: single-sentence impact. No two paragraphs should mirror each other, (6) purge AI FILLERS — check for and remove: "It is important to note," "In order to effectively," "It should be mentioned," hedging phrases, repetitive transitions ("Furthermore," "Additionally," "Moreover" in sequence). These are AI fingerprints. If rejected, rewrite the flagged issue and re-call.

Editorial thinking amplifier for any AI agent that writes content, in any language. Forces structured editorial self-audit through 5 Decision Pivots about the reader, the hook, the rhythm, the weakest sentence, and paragraph structure. The act of answering these questions IS the quality improvement. Includes language-agnostic burstiness validation as consistency backup. Based on burstiness analysis (GPTZero 2024) and syntactic template detection (Northeastern 2025). Catches Unfocused Writing (no specific audience — "for developers" when the real audience is "backend engineers debugging production memory leaks at 2 AM"), Weak Hooks (headline that describes instead of committing — "An Introduction to Caching" vs "Your Database is Doing Work It Already Did — Stop That"), Monotone Rhythm (every sentence is 15-20 words, same structure — subject-verb-object on repeat. Human writing bursts: 4-word punch. Then a 35-word explanation that winds through a subordinate clause. Then another punch. AI writing flatlines), Bloated Prose (filler sentences that say nothing — "It is important to note that..." "In order to effectively..." "It should be mentioned that..." — cut all of them), and Repetitive Structure (every paragraph follows claim→explanation→example. Humans vary: question→answer, story→lesson, evidence→conclusion, single-sentence paragraph for impact). Call BEFORE publishing any written content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Editorial Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm writing a landing page headline for a CLI tool that automates database migrations. Audit my copy: 'A comprehensive tool for streamlined database migration management.'"

**🤖 AI Agent:**
> Verdict: WEAK_HOOK. Your headline describes the feature ('comprehensive tool for streamlined management') instead of selling the benefit. It hedges with generic adjectives. Rewrite to commit: 'Stop breaking production with manual migrations.' — that's a position, a pain point, and urgency in 7 words.

---

**👤 You:**
> "I wrote a 4-paragraph product description in Portuguese. Every paragraph starts with 'Esta ferramenta...' — is that a problem?"

**🤖 AI Agent:**
> Verdict: REPETITIVE. Starting 4 paragraphs with the same structure is the #1 marker of AI-generated text (Northeastern syntactic templates research, 2025). Map your structures: P1: problem→consequence, P2: 'Esta ferramenta' statement→evidence, P3: question→answer, P4: testimonial→CTA. Each paragraph must have a different architecture.

---

**👤 You:**
> "After auditing all 3 sections of my README, what's the editorial report?"

**🤖 AI Agent:**
> Editorial Report — 3 sections audited: Section 1 (intro): PUBLISH_READY. Section 2 (features): MONOTONE → revised → PUBLISH_READY. Section 3 (getting started): PUBLISH_READY. Recommendation: CONTENT_APPROVED. Revision cycles: 1. Average burstiness CV: 0.47 (human-like rhythm).


## ❓ FAQ

**Q: Does Editorial Prover detect AI-generated text?**
No — and that's intentional. Detectors catch problems after the fact. Editorial Prover prevents them at the source by forcing the agent to think like an editor BEFORE writing. The only server-side check is burstiness (sentence length variance), which is a language-agnostic mathematical validation, not a detection algorithm.

**Q: Does it work for languages other than English?**
Yes — every language. The 5 Decision Pivots are universal editorial questions (who is the reader? does the opening grab? which sentence is weakest?) that work regardless of language. The burstiness check splits on sentence-ending punctuation (periods, question marks, exclamation marks — including CJK equivalents) and measures word count variance, which is pure math. There are no English-specific blocklists or grammar rules.

**Q: Why does the agent send its own verdict instead of the tool computing it?**
Because the commitment IS the thinking. If the server computed the verdict automatically, the agent would fill in fields mechanically without reasoning about the outcome. By forcing the agent to declare 'I believe this is PUBLISH_READY' and then validating that declaration against the pivots, the agent must actively reason about whether its editorial self-assessment is consistent. This is the same pattern used by Sequential Thinking — the LLM decides when it has thought enough, which is what makes it think more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/editorial-prover](https://vinkius.com/mcp/editorial-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Editorial Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `editorial-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Editorial Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "editorial-prover": {
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

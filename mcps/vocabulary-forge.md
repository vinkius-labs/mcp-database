# Vocabulary Forge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vocabulary-forge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI detectors don't scan for bad grammar — they scan for vocabulary. "Delve", "leverage", "furthermore" are fingerprints. Vocabulary Forge makes the agent build a complete voice profile: define the person, map tonal shifts, purge signal words, add human roughness, commit to a signature. Any language.

## Description
Every text written by an AI carries invisible fingerprints. Not in grammar — grammar is easy to get right. The fingerprints are in vocabulary: the same 30 words that every model reaches for, the same flat register from start to finish, the same perfect absence of human roughness. AI detectors (GPTZero, Binoculars, DetectGPT) don't look for mistakes. They look for patterns no human produces.

### The Problem It Solves

AI-generated text fails detection for six specific reasons:

- **Voice absence** — the text has no person behind it. It reads as "the AI" talking.
- **Flat register** — same formality throughout. Humans shift: casual opening, technical body, blunt close.
- **AI lexicon** — "delve", "leverage", "furthermore", "tapestry", "landscape", "robust", "comprehensive". These words appear in AI output 10-100x more frequently than in human text.
- **Sterile prose** — zero colloquialisms, perfect grammar everywhere, no contractions, no sentence fragments. Too clean to be human.
- **No identity** — the text could be from anyone. No recurring phrases, no structural tics, no personality.
- **Language blindness** — applying English AI patterns to Portuguese, French, or Japanese content.

Prompting "write like a human" does nothing. The agent still reaches for the same vocabulary. You need to intervene at the vocabulary layer.

### How It Works

Vocabulary Forge uses 5 Decision Pivots that force the agent to construct a complete human-authentic vocabulary profile before writing a single word:

1. **voiceAnchored** — Define a SPECIFIC human voice. Not "professional writer" — a person: age, habits, pet peeves, sentence preferences.
2. **registerMapped** — Map how the tone SHIFTS. At least 3 zones: opening register, body register, closing register. Flat = flagged.
3. **antiVocabularyPurged** — List at least 8 BANNED words. Include known AI signals (delve, leverage, etc.) plus domain overuse. Absence > camouflage.
4. **colloquialismIntegrated** — Add 3+ colloquialisms NATIVE to the target language. Contractions, idioms, discourse markers, sentence fragments.
5. **signatureCommitted** — Define 3+ recurring expressions that fingerprint the voice. Not clichés — unique verbal habits.

The engine validates everything. If your voice description says "professional writer", it rejects — that's a role, not a voice. If your banned list has fewer than 8 words, it rejects. If your register map describes uniform tone, it rejects. If your signatures are business clichés, it rejects.

### The Core Insight: Anti-Vocabulary

The most powerful humanization technique is not adding human words — it's REMOVING AI words. Detectors work by scanning for the presence of signal vocabulary. If those 30-40 words are completely absent from the text, the detector's primary signal vanishes. The anti-vocabulary (banned words list) is the foundation of the entire profile.

### Language-Agnostic by Design

Vocabulary Forge works for any language. The pivots are universal: every language has voices, register shifts, AI-overused words, colloquialisms, and signature patterns. The engine validates depth and consistency — it doesn't prescribe English-specific rules to Portuguese content.


## Available Tools
- **forge_vocabulary**: You must: (1) define a SPECIFIC human voice — not "professional writer" but a person with habits, preferences, and pet peeves, (2) map how the register SHIFTS — flat tone = AI signal, (3) list at least 8 BANNED words — AI detectors scan for "delve", "leverage", "furthermore", "robust", "comprehensive" — absence is your primary defense, (4) integrate COLLOQUIALISMS native to the target language — contractions, idioms, discourse markers, sentence fragments, (5) commit to SIGNATURE expressions — recurring phrases that fingerprint the voice. If the tool rejects, your vocabulary will be detected as AI. Fix the profile.

Structured reflection tool for building human-authentic vocabulary profiles that defeat AI detection. Works in any language. The agent must anchor a specific voice, map register shifts, purge AI-signal words, integrate colloquialisms, and commit to signature expressions before writing anything. The tool validates consistency — if your profile still carries AI lexicon or lacks human roughness, it rejects. Based on detection research: GPTZero (Tian, 2024 — perplexity + burstiness analysis), DetectGPT (Mitchell et al., 2023 — log-probability curvature), Binoculars (Hans et al., 2024 — cross-model perplexity ratio). Catches Voice Absent (writing without a defined human personality — a corporate quarterly report: 2,000 words. Zero contractions. Zero colloquialisms. Every sentence is 18-22 words. No paragraph shorter than 4 lines. "Furthermore, the organization has demonstrated robust growth across comprehensive metrics." GPTZero analysis: 99.2% likely AI-generated. Why: uniform sentence length (low burstiness), formal register sustained without variation, and AI-signal vocabulary ("furthermore," "robust," "comprehensive"). Human writing is IRREGULAR. Sentence length varies: 4 words. Then 37. Then 12. Tone shifts: formal paragraph, then a casual aside, then a one-word reaction. Fix: define a SPECIFIC human voice before writing — not "professional" but a person with habits, preferences, and pet peeves), Flat Register (maintaining the same tone from start to finish — a press release: 47 paragraphs, every single one in the same measured, neutral, corporate voice. No rhetorical question. No imperative. No fragment. No aside. No shift in energy. Humans cannot sustain one register for 47 paragraphs. They get excited, then measured, then blunt, then contemplative. Register variation is the burstiness signal that AI detectors measure. Flat = machine. Varied = human. Fix: map at least 3 tonal zones. Opening: provocative (rhetorical question or bold claim). Body: measured analysis with casual parenthetical asides. Conclusion: blunt imperative or reflective question), AI Lexicon (using words that are statistical markers for AI-generated text — "delve" appears 3× in a 1,500-word article. "Leverage" 4×. "Comprehensive" 6×. "Furthermore" starts 3 paragraphs. "Tapestry" appears metaphorically. These words are not wrong — they are SIGNALS. AI models overuse them relative to human base rates. "Delve" appears 10× more frequently in GPT-4 output than in human-authored articles from the same domain. The anti-vocabulary (words you NEVER use) is more powerful than the vocabulary. Fix: ban at least 8 AI-signal words. Replace with domain-specific alternatives. "Delve into" → "look at." "Leverage" → "use." "Comprehensive" → "thorough" or "complete." "Furthermore" → "Also" or just start the sentence without a connector), Sterile (technically correct but lacking human texture — a travel blog about visiting Lisbon: "Lisbon is a beautiful city with a rich history. The food is excellent. The architecture is impressive. The weather is pleasant." This is a Wikipedia summary, not a human travel story. Human version: "I got lost three times looking for the tram. The map was useless — the streets bend like they were drawn by someone who had too much port wine. Found a bakery by accident. The pastel de nata was still warm. I ate four." Human writing has: specificity (three times, four pastéis), sensory detail (still warm), opinion (map was useless), humor (port wine), and imperfection (got lost). Fix: integrate colloquialisms native to the target language. Contractions. Idioms. Discourse markers. Sentence fragments. Imperfect grammar when natural), and Forgettable (no recurring patterns that fingerprint the voice — an article that could have been written by any competent writer. No recurring phrase. No structural tic. No punctuation habit. Swap the byline to any other author — it reads the same. Human writers have SIGNATURES: Hemingway's short declarative sentences. David Foster Wallace's footnotes. Joan Didion's "We tell ourselves stories in order to live." A newsletter writer who always opens with "Right. So." An analyst who uses em-dashes obsessively — like this — to insert asides. Fix: commit to at least 3 signature expressions. Recurring phrases or structural tics that make this voice recognizable even without the byline). Call once per voice profile, before any content creation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vocabulary Forge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to write a blog post about AI tools. Build me a vocabulary profile that sounds professional and engaging."

**🤖 AI Agent:**
> Verdict: VOICE_ABSENT. "Professional and engaging" is a mood, not a voice. Who is writing this blog post? A former developer turned product manager who writes like she's explaining something to a smart friend over coffee? A cynical journalist who's seen too many AI hype cycles? An enthusiastic CTO who writes in short bursts and uses too many em-dashes? Define the person first.

---

**👤 You:**
> "Voice: cynical tech journalist, mid-30s, hates buzzwords, short punchy sentences. Banned: delve, leverage, comprehensive, robust, furthermore, tapestry, landscape, seamless, utilize, harness, holistic, paradigm. Colloquialisms: look, honestly, here's the thing, don't, can't. Signatures: single-word paragraph closers, question openers, dashes over semicolons. Register: provocative opener, skeptical body, imperative close."

**🤖 AI Agent:**
> Verdict: VOICE_AUTHENTIC. Voice anchored — cynical tech journalist with specific habits (short sentences, periods, dashes). Register mapped — 3 distinct zones (provocative → skeptical → imperative). Anti-vocabulary: 12 banned words including 8 known AI signals. Colloquialisms: 5 discourse markers native to English. Signatures: 3 structural tics (single-word closers, question openers, dash preference). This vocabulary profile defeats detection. Write with it.

---

**👤 You:**
> "Voice: senior product manager who communicates clearly. Register: professional throughout. Banned: delve, leverage. Colloquialisms: none — this is formal writing. Signatures: none needed."

**🤖 AI Agent:**
> Multiple rejections. (1) VOICE_ABSENT — "senior PM who communicates clearly" is a LinkedIn headline, not a voice. (2) FLAT_REGISTER — "professional throughout" is the strongest AI signal. Map 3 zones. (3) AI_LEXICON — only 2 banned words, minimum is 8. (4) STERILE — "none" for colloquialisms = no human roughness. (5) FORGETTABLE — "none needed" for signatures = no identity. Fix all five.


## ❓ FAQ

**Q: Does Vocabulary Forge write content?**
No. Vocabulary Forge generates zero content. It forces the AI agent to build a complete vocabulary PROFILE — voice, register, banned words, colloquialisms, signatures — before writing anything. The profile then guides the agent's word choices. The tool validates the profile's depth and consistency, not the final text.

**Q: What is the anti-vocabulary and why is it the most important part?**
The anti-vocabulary is the list of words the voice MUST NEVER use. AI detectors work by scanning for the presence of ~30-40 signal words that appear in AI output 10-100x more than in human text. If those words are absent, the detector's primary signal disappears. Banning 'delve', 'leverage', 'comprehensive', 'robust', 'furthermore' does more to defeat detection than adding human words. Absence is stronger than camouflage.

**Q: Does it work for languages other than English?**
Yes — any language. The five pivots are universal: every language has human voices, register shifts, AI-overused words, colloquialisms, and signature patterns. The engine validates depth and consistency without prescribing English-specific rules. For Portuguese, ban 'além disso', 'abrangente', 'robusto'. For French, ban 'en outre', 'exhaustif'. For Japanese, identify the keigo/casual register shifts your voice uses. The colloquialisms must be native to the target language.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vocabulary-forge](https://vinkius.com/mcp/vocabulary-forge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vocabulary Forge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vocabulary-forge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vocabulary Forge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vocabulary-forge": {
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

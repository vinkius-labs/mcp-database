# Natural Tokenizer Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/natural-tokenizer-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Tokenize text into words, numbers, emails, URLs, emojis, and hashtags deterministically. AI struggles with mixed content — this engine extracts exact linguistic entities instantly.

## Description
You feed a tweet to an AI and ask it to extract the hashtags and emojis. It uses Byte Pair Encoding (BPE), meaning it sees words as sub-tokens. It frequently hallucinates boundaries, splitting hashtags or merging URLs with punctuation.

This MCP uses `wink-tokenizer` (inspired by Python's spaCy) to perform deterministic NLP tokenization. It understands the structural rules of human language, cleanly separating words from punctuation, while keeping complex entities like emails, URLs, and emojis intact.

### The Superpowers

- **Entity Extraction:** Accurately tags tokens as `word`, `number`, `email`, `url`, `emoji`, `hashtag`, or `mention`.
- **Punctuation Awareness:** Intelligently separates punctuation from words without breaking abbreviations (e.g., 'U.S.A.' stays together, 'End.' splits).
- **Mixed Content Ready:** Flawlessly parses social media posts containing text, links, and emojis mixed together.
- **Deterministic NLP:** Math-based parsing, not LLM probability guessing.


## Available Tools (1)
- **natural_tokenizer**: Tokenize natural language text into exact words, numbers, emails, URLs, emojis, and hashtags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Natural Tokenizer Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract all URLs and hashtags from this Instagram caption."

**🤖 AI Agent:**
> Tokens extracted: 3 URLs, 5 hashtags. Punctuation cleanly separated.

---

**👤 You:**
> "Count how many words and how many emojis are in this chat message log."

**🤖 AI Agent:**
> Statistics: 42 words, 8 emojis, 12 punctuation marks.

---

**👤 You:**
> "Find all the @mentions in this block of customer feedback."

**🤖 AI Agent:**
> Extracted Entities: [@mention] @support, [@mention] @ceo.


## ❓ FAQ

**Q: Why not just use regular expressions (regex)?**
Regex is brittle. A regex for URLs might break if it ends with a period, or fail to handle complex unicode emojis. This engine uses a robust, battle-tested state machine designed specifically for natural language parsing.

**Q: How does it handle abbreviations vs end-of-sentence periods?**
It's smart enough to know that 'Ph.D.' is a single word token, but 'world.' is the word 'world' followed by a punctuation token '.'. This is crucial for accurate sentence boundary detection.

**Q: Can it extract all emails from a large block of text?**
Yes. Pass the text and filter the resulting tokens where tag === 'email'. You'll get an exact array of every email address found, completely separated from surrounding text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/natural-tokenizer-engine](https://vinkius.com/mcp/natural-tokenizer-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Natural Tokenizer Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `natural-tokenizer-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Natural Tokenizer Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "natural-tokenizer-engine": {
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

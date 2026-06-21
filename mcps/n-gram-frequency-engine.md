# N-Gram Frequency Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/n-gram-frequency-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Exact deterministic unigram, bigram, and trigram counting over huge texts. Save tokens and guarantee 100% accurate phrase counts.

## Description
Counting the most frequent 2-word or 3-word phrases (N-Grams) in a 100-page document is an expensive and inaccurate task for an LLM. Due to token limits, LLMs will approximate the counts or miss phrases entirely. The N-Gram Frequency Engine processes the text directly in native V8 JavaScript, delivering mathematically perfect frequency counts for bigrams, trigrams, and custom N-Grams in milliseconds.


## Available Tools (1)
- **extract_ngram_frequencies**: Extracts the top most frequent N-Grams (e.g. bigrams, trigrams) from a text deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **N-Gram Frequency Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here is a 50-page PDF text. Find the top 10 most frequent trigrams (n=3) to help me understand the core topics."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Combine all these customer reviews into one string and extract the top 5 bigrams (n=2)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Extract the exact frequencies of 4-grams from this competitor's article to map their SEO keyword strategy."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: What are Bigrams and Trigrams?**
A bigram is a sequence of two adjacent words (e.g., 'machine learning'). A trigram is three (e.g., 'natural language processing').

**Q: Does it lowercase the text automatically?**
Yes, all text is automatically lowercased and tokenized natively to ensure accurate aggregation of phrases.

**Q: Is this faster than asking Claude?**
Significantly faster and 100% accurate. LLMs cannot count occurrences across thousands of tokens reliably.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/n-gram-frequency-engine](https://vinkius.com/mcp/n-gram-frequency-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **N-Gram Frequency Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `n-gram-frequency-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **N-Gram Frequency Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "n-gram-frequency-engine": {
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

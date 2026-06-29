# Keyword Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keyword-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Extract and rank significant keywords from text using term frequency and density analysis.

## Description
The Keyword Extractor is an analytical engine designed to identify the most relevant terms within any provided text. By utilizing Term Frequency (TF) and keyword density calculations, it filters out linguistic noise using hardcoded stopword lists for English, Portuguese, and Spanish. You can use `rank_keywords` to get a prioritized list of terms, `calculate_term_density` to investigate the prevalence of a specific word, or `verify_language_capability` to check supported languages.


## Available Tools (3)
- **calculate_term_density**: Analyzes a specific word's importance within a given text block
- **rank_keywords**: Provides a prioritized list of keywords found within a text
- **verify_language_capability**: Confirms whether the requested language is available


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keyword Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the most important keywords from this text: 'The quick brown fox jumps over the lazy dog. The dog was very lazy.' using English."

**🤖 AI Agent:**
> The top keywords are: fox (1), quick (1), brown (1), jumps (1), over (1), lazy (2), dog (2).

---

**👤 You:**
> "What is the density of the word 'apple' in this text: 'Apple is a fruit. I love eating apple every day.' using English?"

**🤖 AI Agent:**
> The term 'apple' was found 2 times, with a calculated density of 0.5.

---

**👤 You:**
> "Is Spanish supported for keyword extraction?"

**🤖 AI Agent:**
> Yes, Spanish (es) is a supported language.


## ❓ FAQ

**Q: Which languages are supported?**
The engine currently supports English (en), Portuguese (pt), and Spanish (es) through hardcoded stopword lists.

**Q: How is keyword density calculated?**
Density is calculated by dividing the frequency of a specific term by the total count of all valid tokens (words that are not stopwords) in the text.

**Q: Can I check if a language is supported before running analysis?**
Yes, you can use the `verify_language_capability` tool to confirm if a specific ISO 63                639-1 code is available for extraction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keyword-extractor](https://vinkius.com/mcp/keyword-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keyword Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keyword-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keyword Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keyword-extractor": {
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

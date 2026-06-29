# LSI Keyword Finder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lsi-keyword-finder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [seo](../categories/seo.md)

Extract semantically related keywords using co-occurrence, synonyms, and morphological variations.

## Description
LSI Keyword Finder is a semantic extraction engine designed to identify meaningful terms within text. By analyzing `extract_core_keywords`, the tool identifies significant words based on frequency and stop-word filtering. The `expand_keyword_network` tool builds connections between words using co-occurrence analysis and pre-defined synonym mappings. Additionally, `get_word_variations` allows you to find morphological variants like singular and plural forms. This engine provides a deterministic way to understand semantic relationships without external API dependencies.


## Available Tools (3)
- **expand_keyword_network**: Generates a list of semantically related keywords for a specific seed word
- **extract_core_keywords**: Identifies the most significant and frequent meaningful terms within a provided body of text
- **get_word_variations**: Identifies all known morphological variations for a given input


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LSI Keyword Finder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the most important keywords from this text: 'The quick brown fox jumps over the lazy dog. The dog was very happy.'"

**🤖 AI Agent:**
> ["quick", "brown", "fox", "jumps", "lazy", "dog"]

---

**👤 You:**
> "Find keywords related to 'apple' in the context: 'I ate a delicious red apple while sitting under the apple tree.'"

**🤖 AI Agent:**
> ["delicious", "red", "tree"]

---

**👤 You:**
> "What are the variations of the word 'keyword'?"

**🤖 AI Agent:**
> ["keywords"]


## ❓ FAQ

**Q: How does the keyword extraction work?**
The `extract_core_keywords` tool processes your text by removing common stop words and then counting the frequency of the remaining terms. You can set a minimum frequency threshold to filter out less significant words.

**Q: Can I find synonyms for a specific word?**
Yes, you can use `expand_keyword_network` which leverages both synonym mapping and co-occurrence within your provided context text.

**Q: How are morphological variations handled?**
The `get_word_variations` tool looks up the input word in a morphology registry to identify all known grammatical variants, such as singular and plural forms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lsi-keyword-finder](https://vinkius.com/mcp/lsi-keyword-finder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LSI Keyword Finder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lsi-keyword-finder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LSI Keyword Finder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lsi-keyword-finder": {
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

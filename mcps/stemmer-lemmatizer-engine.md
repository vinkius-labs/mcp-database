# Stemmer & Lemmatizer Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stemmer-lemmatizer-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Porter and Lancaster local text stemming. Reduce vocabulary size exactly and deterministically before feeding text to a vector database.

## Description
Stemming reduces words to their root or base form (e.g., 'running' to 'run'). This is critical for preparing text for vector search, RAG, or topic modeling. Rather than asking an LLM to manually stem thousands of words (which wastes tokens and risks semantic alteration), this engine applies mathematically proven Porter or Lancaster algorithms natively local to clean and reduce your entire text corpus in one fast operation.


## Available Tools
- **stem_text_corpus**: Applies Porter or Lancaster stemming algorithms to tokenize and stem text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stemmer & Lemmatizer Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take this long customer review and apply Porter stemming so I can use it for clustering."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Stem these database entries using the Lancaster algorithm to compress the vocabulary size."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Before we send this text to the embedding model, run it through the stemmer tool to normalize all verbs and plurals."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: Porter vs Lancaster?**
Porter is gentler and more common. Lancaster is aggressive and creates much shorter stems (sometimes stripping prefixes/suffixes completely).

**Q: Does it help with RAG?**
Yes! Stemming documents before embedding them reduces vector dimensionality and increases recall for different word variations.

**Q: Does it do tokenization?**
Yes, it automatically tokenizes the string, stems each word, and rejoins them for your convenience.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stemmer-lemmatizer-engine](https://vinkius.com/mcp/stemmer-lemmatizer-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stemmer & Lemmatizer Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stemmer-lemmatizer-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stemmer & Lemmatizer Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stemmer-lemmatizer-engine": {
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

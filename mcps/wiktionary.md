# Wiktionary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wiktionary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Universal linguistic intelligence — get word definitions, etymologies, and examples via AI.

## Description
Equip your AI agent with the power of the world's most comprehensive collaborative dictionary through the **Wiktionary** MCP server. This integration provides instant access to linguistic data for thousands of words and phrases. Your agent can retrieve precise definitions, identify parts of speech (nouns, verbs, adjectives), see usage examples, and get concise summaries for encyclopedic topics. Whether you are improving your writing, translating complex texts, or exploring etymology, your agent acts as a dedicated philologist and lexicographer through natural conversation.

### What you can do

- **Word Definitions** — Retrieve detailed linguistic definitions and parts of speech.
- **Encyclopedic Summaries** — Get concise descriptions for words that also function as general topics.
- **Linguistic Examples** — View real-world usage examples for better understanding of context.
- **Multilingual Support** — Access definitions and data across various languages supported by the platform.
- **Etymology Auditing** — Explore the history and origin of words across different linguistic roots.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying word data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Editors** — verify word meanings and find the perfect term for any context.
- **Language Learners** — explore definitions and parts of speech to build vocabulary.
- **Translators** — access a reliable source for cross-linguistic reference.
- **Researchers** — retrieve structured linguistic data for academic or professional projects.


## Available Tools
- **get_word_definition**: Get the definition of a word
- **get_word_summary**: Get a short summary of a word or topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wiktionary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the definition of the word 'ephemeral'?"

**🤖 AI Agent:**
> The word 'ephemeral' is an adjective meaning lasting for a very short time. For example: 'ephemeral pleasures'. Would you like to see more definitions or examples?

---

**👤 You:**
> "Give me a summary of 'Computer Science'."

**🤖 AI Agent:**
> Retrieving summary... Computer science is the study of computation, information, and automation. It spans theoretical disciplines to applied disciplines. Would you like the full definition or related terms?

---

**👤 You:**
> "Identify the part of speech for 'serendipity'."

**🤖 AI Agent:**
> Analyzing... 'Serendipity' is a noun. It refers to the occurrence and development of events by chance in a happy or beneficial way. I can provide examples of how to use it in a sentence.


## ❓ FAQ

**Q: Can I get the definition of an obscure word like 'synecdoche'?**
Yes! Use the `get_word_definition` tool with the word 'synecdoche'. It will return the definitions, examples, and the part of speech from Wiktionary.

**Q: How do I see the part of speech for a word?**
The `get_word_definition` tool automatically identifies if a word is a noun, verb, adjective, etc., and provides definitions for each relevant part of speech.

**Q: Does it provide a summary for general topics?**
Yes. Use the `get_word_summary` tool to retrieve a concise description of a word that also functions as an encyclopedic topic, suitable for quick overviews.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wiktionary](https://vinkius.com/mcp/wiktionary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wiktionary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wiktionary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wiktionary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wiktionary": {
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

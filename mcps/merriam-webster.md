# Merriam-Webster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/merriam-webster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Official Merriam-Webster dictionary and thesaurus — access definitions and synonyms via AI.

## Description
Equip your AI agent with the gold standard of the English language via the **Merriam-Webster** MCP server. This integration provides your agent with instant access to the prestigious Collegiate Dictionary and Thesaurus. Your agent can instantly fetch precise definitions, audit etymologies, and retrieve comprehensive synonym/antonym lists without you ever needing to browse a physical dictionary or website. Whether you are refining your writing or verifying technical linguistic nuances, your agent acts as a dedicated lexicographer through natural conversation.

### What you can do

- **Word Definitions** — Retrieve detailed definitions, parts of speech, and pronunciations for thousands of English words.
- **Thesaurus Auditing** — Fetch extensive lists of synonyms, antonyms, and related words to enrich your vocabulary.
- **Usage Examples** — Access authentic sentence examples to understand how words are used in real-world contexts.
- **Linguistic Intelligence** — Verify the correct spelling and grammatical category of complex terms.
- **Discovery** — Identify related words and linguistic patterns through aggregate search results.

### How it works

1. Subscribe to this server
2. Enter your Merriam-Webster Dictionary and Thesaurus API Keys
3. Start managing your linguistic intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Editors** — instantly find the perfect word and verify definitions during the creative process.
- **Students & Language Learners** — explore the nuances of English vocabulary and usage through an AI-guided interface.
- **Content Creators** — retrieve synonyms and usage examples to polish scripts, articles, and social media posts.
- **IT & Legal Professionals** — verify the precise meaning of technical and formal terminology.
- **Developers** — integrate reliable linguistic data into their applications through natural language queries.


## Available Tools
- **define_word**: Get the definition of a word
- **get_thesaurus**: Get synonyms and antonyms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Merriam-Webster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Define the word 'serendipity'."

**🤖 AI Agent:**
> Retrieving the definition for 'serendipity'... It is a noun referring to the faculty or phenomenon of finding valuable or agreeable things not sought for. Would you like to see usage examples?

---

**👤 You:**
> "Find synonyms for 'eloquent' in the Merriam-Webster thesaurus."

**🤖 AI Agent:**
> Searching for synonyms of 'eloquent'... I've found several related words including 'articulate', 'fluent', and 'silver-tongued'. I can also list antonyms if you're interested.

---

**👤 You:**
> "What is the origin of the word 'lexicographer'?"

**🤖 AI Agent:**
> Fetching etymology for 'lexicographer'... The term comes from the Greek 'lexikon' (dictionary) and 'graphos' (writer). It literally means a writer of dictionaries. Should I check its specific definition in the dictionary?


## ❓ FAQ

**Q: Do I need separate API keys for the dictionary and thesaurus?**
Yes, Merriam-Webster provides separate keys for the Collegiate Dictionary and the Collegiate Thesaurus. You must provide both in the credentials section to enable all tools.

**Q: What happens if a word is not found?**
If an exact match is not found, the API often returns a list of suggestions. Your agent will display these suggestions to help you find the correct term.

**Q: Can I see the part of speech for a word?**
Yes! Every definition returned by the `define_word` tool includes the part of speech (e.g., noun, verb, adjective) next to the word headword.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/merriam-webster](https://vinkius.com/mcp/merriam-webster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Merriam-Webster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `merriam-webster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Merriam-Webster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "merriam-webster": {
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

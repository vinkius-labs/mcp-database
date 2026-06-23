# DictionaryAPI.dev MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dictionaryapidev)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access comprehensive English word definitions, phonetics, and usage examples directly through your AI agent.

## Description
Integrate the **Free Dictionary API** into your AI workflows to provide instant, accurate linguistic data. This server allows any MCP-compatible agent to look up English words, retrieve multiple definitions, explore etymology, and hear phonetic pronunciations.

### What you can do

- **Word Definitions** — Get clear, structured meanings for any English word across various parts of speech.
- **Phonetics** — Access IPA transcriptions and audio links to understand correct pronunciation.
- **Usage Examples** — See how words are used in real-world sentences to better understand context and nuance.
- **Synonyms & Antonyms** — Expand your vocabulary with related terms provided directly in the API response.

### How it works

1. Subscribe to this server
2. No API key or complex configuration is required
3. Start querying definitions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Editors** — instantly verify definitions and find synonyms without leaving your drafting environment.
- **Language Learners** — get immediate context and phonetic help while reading or writing in English.
- **Developers** — integrate linguistic data into your prompts for better content generation or data labeling.


## Available Tools (1)
- **get_word_definition**: Get definitions, phonetics, and origins for an English word


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DictionaryAPI.dev** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the definition and phonetics for the word 'ephemeral'."

**🤖 AI Agent:**
> I've looked up 'ephemeral'. It is an adjective meaning 'lasting for a very short time'. The phonetic pronunciation is /əˈfɛmərəl/. Would you like to see some usage examples?

---

**👤 You:**
> "What are the different meanings of the word 'bark'?"

**🤖 AI Agent:**
> The word 'bark' has multiple meanings: 1. The sharp explosive cry of a dog. 2. The tough protective outer sheath of the trunk and branches of a tree. 3. To utter a command abruptly. Which context are you interested in?

---

**👤 You:**
> "Find synonyms for the word 'innovative' using the dictionary."

**🤖 AI Agent:**
> For 'innovative', the dictionary suggests synonyms such as: 'original', 'groundbreaking', 'pioneering', and 'state-of-the-art'.


## ❓ FAQ

**Q: Does this server support languages other than English?**
Currently, the `get_word_definition` tool is optimized for the English language as provided by the DictionaryAPI.dev source.

**Q: Can I retrieve synonyms and antonyms for a word?**
Yes. When the API has related terms available, the `get_word_definition` tool will include them in the response alongside the definitions.

**Q: Is there a limit to how many words I can look up?**
The server uses the public DictionaryAPI.dev service. While it is free and open, it is intended for fair use. The `get_word_definition` tool handles standard lookup requests efficiently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dictionaryapidev](https://vinkius.com/mcp/dictionaryapidev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DictionaryAPI.dev** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dictionaryapidev` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DictionaryAPI.dev** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dictionaryapidev": {
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

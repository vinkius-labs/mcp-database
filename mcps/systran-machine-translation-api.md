# Systran (Machine Translation API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/systran-machine-translation-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Professional machine translation and linguistic analysis via Systran — translate text, detect languages, and perform dictionary lookups.

## Description
Connect to **Systran**, the pioneer in machine translation, to empower your AI agent with high-quality translation and linguistic analysis capabilities through natural conversation.

### What you can do

- **Text Translation** — Translate strings or arrays of text between dozens of languages with support for HTML and annotations.
- **Document Translation** — Submit file content for translation while preserving the original formatting and structure.
- **Language Detection** — Automatically identify the source language of any given text with high confidence.
- **Dictionary Lookup** — Access professional or user-defined dictionaries for precise term definitions and translations.
- **Morphological Analysis** — Extract grammatical information, parts of speech, and word forms for deep linguistic processing.

### How it works

1. Subscribe to this server
2. Enter your Systran API Key
3. Start translating and analyzing text directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Teams** — quickly translate content strings and verify terminology across multiple languages.
- **Developers** — integrate professional translation and language detection directly into your coding workflow.
- **Researchers & Analysts** — perform deep linguistic analysis and morphological extraction on foreign language texts.


## Available Tools (5)
- **detect_language**: Identify the language of a given text
- **dictionary_lookup**: Look up terms in Systran or user-defined dictionaries
- **extract_morphology**: Extract morphological information from text
- **translate_file**: Returns a requestId to track the asynchronous translation task.

Translate documents while preserving formatting
- **translate_text**: Use "auto" for the source language to automatically detect it.

Translate text from a source language to a target language


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Systran (Machine Translation API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate the following sentences to French: ['Hello world', 'How are you today?']"

**🤖 AI Agent:**
> I've translated your text using Systran. The results are: 'Bonjour le monde' and 'Comment allez-vous aujourd'hui ?'.

---

**👤 You:**
> "Identify the language of this text: 'Guten Tag, wie kann ich Ihnen helfen?'"

**🤖 AI Agent:**
> The `detect_language` tool identified this text as German (de).

---

**👤 You:**
> "Look up the term 'cloud computing' in the English to Spanish dictionary."

**🤖 AI Agent:**
> Performing dictionary lookup... For 'cloud computing', the Spanish translation is 'computación en la nube'. It is categorized as a technical noun.


## ❓ FAQ

**Q: Can I translate HTML content while preserving the tags?**
Yes! Use the `translate_text` tool and set the `format` parameter to 'html'. The engine will translate the text content while keeping your HTML structure intact.

**Q: How do I find the specific meaning of a technical term in another language?**
Use the `dictionary_lookup` tool. Provide the term in the `input` field along with the `source` and `target` language codes to get professional dictionary definitions and translations.

**Q: Can the AI identify a language if I don't know what it is?**
Absolutely. Use the `detect_language` tool with any text input. The server will return the detected language code and confidence level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/systran-machine-translation-api](https://vinkius.com/mcp/systran-machine-translation-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Systran (Machine Translation API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `systran-machine-translation-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Systran (Machine Translation API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "systran-machine-translation-api": {
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

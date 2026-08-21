# Singlish Formality Translator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singlish-formality-translator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [language](../categories/language.md)

Converts Singlish to Standard English with formality analysis.

## Description
This MCP server provides a deterministic engine to translate Singlish colloquialisms into Standard English. It quantifies the shift in professional tone using formality scores and detects emotional sarcasm markers. Use `translate_singlish` to convert phrases, `get_translation_map` to view the dictionary, or `analyze_formality_components` to identify specific linguistic drivers of formality.


## Available Tools (3)
- **analyze_formality_components**: Breaks down a text to identify which specific words are driving the formality score
- **get_translation_map**: Retrieves the current dictionary of Singlish-to-English phrase mappings
- **translate_singlish**: Converts a Singlish input string into a standardized English equivalent and provides a linguistic formality analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singlish Formality Translator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Translate this: Don't play play"

**🤖 AI Agent:**
> Please take this seriously.

---

**👤 You:**
> "Can or not?"

**🤖 AI Agent:**
> Is this feasible?

---

**👤 You:**
> "Sian, wah lau."

**🤖 AI Agent:**
> I am feeling burnt out.


## ❓ FAQ

**Q: How does the formality score work?**
The score ranges from 0 to 100. Singlish is treated as low-formality (near 0), while Standard English is high-formality (near 100). The `formality_loss` shows the increase in professional tone.

**Q: Can I see the list of supported phrases?**
Yes, you can use the `get_translation_map` tool to retrieve the current dictionary of Singlish-to-English mappings.

**Q: What is sarcasm detection?**
The engine identifies specific Singlish interjections like 'wah lau' or 'aiyo' to flag if the input contains sarcasm markers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singlish-formality-translator](https://vinkius.com/ai-agent-connect/singlish-formality-translator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singlish Formality Translator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singlish-formality-translator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singlish Formality Translator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singlish-formality-translator": {
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

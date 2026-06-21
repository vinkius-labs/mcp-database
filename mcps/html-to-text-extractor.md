# HTML to Text Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-to-text-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Stop wasting AI context on messy HTML code. Instantly strip CSS, tags, and scripts to extract perfectly readable Plain Text.

## Description
When an AI Agent accesses an API like Zendesk or Gmail to read an email, it often receives a massive 3MB HTML string full of inline CSS and broken tables. Forcing the LLM to read this burns thousands of tokens and confuses the AI. This MCP solves that entirely.

### The Superpowers

- **Token Saver:** Converts complex HTML into readable plain text instantly, saving up to 95% of your LLM context window.
- **Smart Formatting:** Preserves spatial layout, lists, and links so the LLM still understands the structure of the original email.


## Available Tools (1)
- **extract_text**: Pass the raw HTML and receive a clean plain-text string without any markup.

Strips raw HTML into clean Plain Text instantly. Reduces token usage by 95% when agents need to read heavy HTML emails or webpages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML to Text Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the text from this messy HTML email before I summarize it."

**🤖 AI Agent:**
> Extracted Text: Returned clean plain text successfully.

---

**👤 You:**
> "Convert this raw HTML page snippet into plain text."

**🤖 AI Agent:**
> Extracted Text: HTML tags removed, layout preserved.

---

**👤 You:**
> "Strip all the tables and CSS from this HTML string."

**🤖 AI Agent:**
> Extracted Text: Stripped output generated.


## ❓ FAQ

**Q: Does it keep the links?**
By default, it drops the raw hrefs to save tokens, but preserves the text of the link.

**Q: Will it extract text from images?**
No, it strips `<img>` tags completely. It does not perform OCR.

**Q: Is it safe against malicious scripts?**
Yes, `<script>` tags and their contents are completely ignored and stripped from the final text.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-to-text-extractor](https://vinkius.com/mcp/html-to-text-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTML to Text Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `html-to-text-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTML to Text Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html-to-text-extractor": {
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

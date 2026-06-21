# HTML XSS Sanitizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-xss-sanitizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Protect your database from malicious code. Clean and sanitize user-generated HTML payloads instantly local.

## Description
If you ask an AI to 'clean this HTML before saving it', it will likely fail to catch obfuscated XSS vectors hidden in Base64 or obscure event handlers. LLMs do not have native rendering engines to test payloads. This MCP provides an enterprise-grade security shield for agents that handle public inputs.

### The Superpowers

- **Surgical Cleaning:** Uses `sanitize-html` to strip dangerous tags (`<script>`, `<iframe>`) and malicious `onload` events.
- **Zero-Trust Input:** Enforces a strict whitelist of safe tags, ensuring that what goes into your database cannot execute harmful code in a browser.


## Available Tools (1)
- **sanitizeHtml_html**: Pass the raw HTML and receive clean, safe HTML with dangerous tags and attributes stripped.

Strips malicious XSS vectors and unsafe tags from HTML payloads before they are saved to a database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTML XSS Sanitizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sanitize this HTML input: `<p>Hello</p><script>alert('hack');</script>`"

**🤖 AI Agent:**
> ✅ **Sanitized HTML:** `<p>Hello</p>`

---

**👤 You:**
> "Clean this blog post content to ensure no malicious iframes are present."

**🤖 AI Agent:**
> ✅ **Cleaned:** Stripped 2 `iframe` tags and 1 `onload` event successfully.

---

**👤 You:**
> "Check if this user comment contains any XSS vectors before we save it."

**🤖 AI Agent:**
> ✅ **Sanitized Payload:** Returned safe string.


## ❓ FAQ

**Q: Does it remove CSS?**
By default, it removes unsafe styles but leaves the structure intact.

**Q: Is it better than asking the LLM to do it?**
Absolutely. LLMs are easily bypassed by obfuscated XSS payloads. This engine relies on strict deterministic whitelisting.

**Q: Are images allowed?**
Yes, `<img>` tags are whitelisted, but only with safe attributes like `src` and `alt`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-xss-sanitizer](https://vinkius.com/mcp/html-xss-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTML XSS Sanitizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `html-xss-sanitizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTML XSS Sanitizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html-xss-sanitizer": {
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

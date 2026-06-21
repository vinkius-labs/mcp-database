# HTML XSS Sanitizer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html-xss-sanitizer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/html-xss-sanitizer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/html-xss-sanitizer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Protect your database from malicious code. Clean and sanitize user-generated HTML payloads instantly local.

## Description
If you ask an AI to 'clean this HTML before saving it', it will likely fail to catch obfuscated XSS vectors hidden in Base64 or obscure event handlers. LLMs do not have native rendering engines to test payloads. This MCP provides an enterprise-grade security shield for agents that handle public inputs.

### The Superpowers

- **Surgical Cleaning:** Uses `sanitize-html` to strip dangerous tags (`<script>`, `<iframe>`) and malicious `onload` events.
- **Zero-Trust Input:** Enforces a strict whitelist of safe tags, ensuring that what goes into your database cannot execute harmful code in a browser.


## Available Tools
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


## Installation & Usage

To install and use the **HTML XSS Sanitizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-xss-sanitizer](https://vinkius.com/mcp/html-xss-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

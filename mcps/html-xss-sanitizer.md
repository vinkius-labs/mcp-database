# HTML XSS Sanitizer MCP Server

Protect your database from malicious code. Clean and sanitize user-generated HTML payloads instantly local.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/html-xss-sanitizer)

## Overview
**Category:** fort-knox
**Tools Count:** 1

## Description
If you ask an AI to 'clean this HTML before saving it', it will likely fail to catch obfuscated XSS vectors hidden in Base64 or obscure event handlers. LLMs do not have native rendering engines to test payloads. This MCP provides an enterprise-grade security shield for agents that handle public inputs.

### The Superpowers

- **Surgical Cleaning:** Uses `sanitize-html` to strip dangerous tags (`<script>`, `<iframe>`) and malicious `onload` events.
- **Zero-Trust Input:** Enforces a strict whitelist of safe tags, ensuring that what goes into your database cannot execute harmful code in a browser.


## Available Tools
- **sanitizeHtml_html**: Pass the raw HTML and receive clean, safe HTML with dangerous tags and attributes stripped.

Strips malicious XSS vectors and unsafe tags from HTML payloads before they are saved to a database


## Installation & Usage

To install and use the **HTML XSS Sanitizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html-xss-sanitizer](https://vinkius.com/mcp/html-xss-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

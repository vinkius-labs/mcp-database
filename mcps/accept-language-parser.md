# Accept Language Parser MCP Server

Parse HTTP Accept-Language headers into priority-ordered language preferences with quality weights.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accept-language-parser)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
When a global routing agent reads `Accept-Language: en-US,pt-BR;q=0.9,fr;q=0.8`, it needs to correctly parse quality weights and determine the user's preferred language. This MCP does it deterministically.

### The Superpowers

- **RFC 7231 Compliant:** Parses quality values (q-factors) exactly as specified by the HTTP standard.
- **Priority Ordered:** Returns languages sorted by quality weight, with the preferred language first.


## Available Tools
- **parse_accept_language**: Pass the raw header value (e.g. "en-US,pt-BR;q=0.9,fr;q=0.8") and receive a priority-ordered list of languages with their quality weights. Never try to parse quality weights manually.

Parses HTTP Accept-Language headers into an ordered list of user language preferences with quality weights. Essential for global routing and i18n agents


## Installation & Usage

To install and use the **Accept Language Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accept-language-parser](https://vinkius.com/mcp/accept-language-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

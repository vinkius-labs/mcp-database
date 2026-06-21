# Accept Language Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accept-language-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/accept-language-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/accept-language-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Parse HTTP Accept-Language headers into priority-ordered language preferences with quality weights.

## Description
When a global routing agent reads `Accept-Language: en-US,pt-BR;q=0.9,fr;q=0.8`, it needs to correctly parse quality weights and determine the user's preferred language. This MCP does it deterministically.

### The Superpowers

- **RFC 7231 Compliant:** Parses quality values (q-factors) exactly as specified by the HTTP standard.
- **Priority Ordered:** Returns languages sorted by quality weight, with the preferred language first.


## Available Tools
- **parse_accept_language**: Pass the raw header value (e.g. "en-US,pt-BR;q=0.9,fr;q=0.8") and receive a priority-ordered list of languages with their quality weights. Never try to parse quality weights manually.

Parses HTTP Accept-Language headers into an ordered list of user language preferences with quality weights. Essential for global routing and i18n agents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accept Language Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this Accept-Language header: en-US,pt-BR;q=0.9,fr;q=0.8"

**🤖 AI Agent:**
> Preferred: en-US (q=1) > pt-BR (q=0.9) > fr (q=0.8)

---

**👤 You:**
> "What is the user's preferred language from: de,en-GB;q=0.7,ja;q=0.3"

**🤖 AI Agent:**
> Preferred: de (q=1, German)

---

**👤 You:**
> "How many languages does the browser support based on this header: zh-CN,zh;q=0.9,en;q=0.8,ko;q=0.7,ar;q=0.6"

**🤖 AI Agent:**
> 5 languages detected: zh-CN, zh, en, ko, ar


## Installation & Usage

To install and use the **Accept Language Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accept-language-parser](https://vinkius.com/mcp/accept-language-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

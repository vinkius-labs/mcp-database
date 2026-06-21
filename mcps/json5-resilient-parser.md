# JSON5 Resilient Parser MCP Server

Parse malformed JSON with trailing commas, comments, and single quotes into perfect strict JSON. Powered by JSON5 (32M+ weekly downloads).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/json5-resilient-parser)

## Overview
**Category:** loved-by-devs
**Tools Count:** 1

## Description
LLMs consistently generate JSON with trailing commas, inline comments, and single quotes. JSON.parse() breaks every time. This MCP catches it all and outputs perfect RFC 8259 JSON.

### The Superpowers

- **Resilient:** Accepts trailing commas, comments (// and /**/), single quotes, unquoted keys, hex numbers, and Infinity/NaN.
- **Strict Output:** Always returns valid RFC 8259 JSON that any parser can consume without modification.


## Available Tools
- **parse_json5**: parse(). The engine accepts any JSON5-compliant string and returns strict RFC 8259 JSON. Essential for cleaning LLM-generated configs.

Parses malformed JSON with trailing commas, comments, single quotes, and unquoted keys — then outputs perfect strict JSON. Powered by JSON5 (32M+ weekly downloads)


## Installation & Usage

To install and use the **JSON5 Resilient Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json5-resilient-parser](https://vinkius.com/mcp/json5-resilient-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

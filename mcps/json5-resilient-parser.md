# JSON5 Resilient Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json5-resilient-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/json5-resilient-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/json5-resilient-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Parse malformed JSON with trailing commas, comments, and single quotes into perfect strict JSON. Powered by JSON5 (32M+ weekly downloads).

## Description
LLMs consistently generate JSON with trailing commas, inline comments, and single quotes. JSON.parse() breaks every time. This MCP catches it all and outputs perfect RFC 8259 JSON.

### The Superpowers

- **Resilient:** Accepts trailing commas, comments (// and /**/), single quotes, unquoted keys, hex numbers, and Infinity/NaN.
- **Strict Output:** Always returns valid RFC 8259 JSON that any parser can consume without modification.


## Available Tools
- **parse_json5**: parse(). The engine accepts any JSON5-compliant string and returns strict RFC 8259 JSON. Essential for cleaning LLM-generated configs.

Parses malformed JSON with trailing commas, comments, single quotes, and unquoted keys — then outputs perfect strict JSON. Powered by JSON5 (32M+ weekly downloads)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON5 Resilient Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this JSON with trailing commas and comments: {name: 'Alice', age: 30, // years old}"

**🤖 AI Agent:**
> Strict JSON Output: {"name": "Alice", "age": 30}

---

**👤 You:**
> "Clean up this LLM-generated config that has single quotes and trailing commas."

**🤖 AI Agent:**
> Strict JSON Output: Clean RFC 8259 JSON generated.

---

**👤 You:**
> "Convert this JSON5 with hex values and Infinity to strict JSON."

**🤖 AI Agent:**
> Strict JSON Output: All values normalized to standard JSON types.


## Installation & Usage

To install and use the **JSON5 Resilient Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json5-resilient-parser](https://vinkius.com/mcp/json5-resilient-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

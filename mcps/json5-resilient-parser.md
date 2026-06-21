# JSON5 Resilient Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json5-resilient-parser)
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


## ❓ FAQ

**Q: What makes this different from JSON.parse()?**
JSON.parse() rejects trailing commas, comments, single quotes, and unquoted keys. JSON5 accepts all of these and outputs strict RFC 8259 JSON.

**Q: Does it support JavaScript-style comments?**
Yes. Both single-line (//) and multi-line (/* */) comments are supported and stripped from the output.

**Q: Can it handle unquoted object keys?**
Yes. `{name: 'Alice'}` is valid JSON5 and will be converted to `{"name": "Alice"}` in the strict output.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json5-resilient-parser](https://vinkius.com/mcp/json5-resilient-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON5 Resilient Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `json5-resilient-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON5 Resilient Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json5-resilient-parser": {
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

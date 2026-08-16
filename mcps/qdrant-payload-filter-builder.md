# Qdrant Payload Filter Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/qdrant-payload-filter-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [database](../categories/database.md)

Convert MongoDB-style filters to valid Qdrant JSON payload structures.

## Description
The Qdrant Payload Filter Builder acts as a structural guardrail for AI agents. It translates MongoDB-style filter dictionaries (using $gt, $lt, and $eq) into the strict Qdrant 'must' array format. Use `generate_qdrant_filter` to create valid JSON, `validate_operator_syntax` to check for unsupported operators, and `analyze_filter_complexity` to evaluate query depth.


## Available Tools (3)
- **analyze_filter_complexity**: Analyzes the computational complexity of a Qdrant filter
- **generate_qdrant_filter**: Generates a Qdrant filter payload from a JSON specification
- **validate_operator_syntax**: Validates the syntax of a specific Qdrant operator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qdrant Payload Filter Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this filter to Qdrant: {category: 'electronics', price: {$gt: 50}}"

**🤖 AI Agent:**
> [{"key": "category", "match": {"value": "electronics"}}, {"key": "price", "range": {"gt": 50}}]

---

**👤 You:**
> "Is this filter syntax clean? `{status: {$eq: 'active'}}`"

**🤖 AI Agent:**
> The syntax is clean; no unsupported operators were found.

---

**👤 You:**
> "What is the complexity of this filter: `{price: {$gt: 10}, color: 'red'}`"

**🤖 AI Agent:**
> The nesting depth is 1 and there are 2 total criteria.


## ❓ FAQ

**Q: How do I use this with Qdrant?**
Use `generate_qdrant_filter` by providing a dictionary like `{price: {$gt: 10}}`.

**Q: What operators are supported?**
The tool supports `$eq`, `$gt`, and `$lt`.

**Q: Can it detect errors?**
Yes, `validate_operator_syntax` identifies unsupported MongoDB operators.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/qdrant-payload-filter-builder](https://vinkius.com/ai-agent-connect/qdrant-payload-filter-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qdrant Payload Filter Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qdrant-payload-filter-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qdrant Payload Filter Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qdrant-payload-filter-builder": {
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

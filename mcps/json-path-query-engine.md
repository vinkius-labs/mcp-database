# JSON Path Query Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-path-query-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Extract specific data from massive JSON payloads using JSONPath expressions.

## Description
Surgically extract fields from complex API responses using JSONPath Plus (8M+ weekly downloads). Saves tokens and prevents hallucination.

### The Superpowers

- **Surgical Extraction:** Full JSONPath syntax (`$.orders[0].total_price`, `$..email`).
- **Token Efficient:** Extract only the 3 fields you need from a 5,000-token payload.


## Available Tools (1)
- **query_json**: Pass the raw JSON string and a JSONPath expression like "$.orders[0].total_price" or "$.users[*].email". Returns all matching values.

Queries and extracts specific values from massive JSON payloads using JSONPath expressions. Eliminates the need to send entire API responses to the LLM context window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Path Query Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract all author names from this bookstore JSON."

**🤖 AI Agent:**
> JSONPath Result: 4 matches found.


## ❓ FAQ

**Q: What JSONPath syntax is supported?**
Full JSONPath Plus: root ($), deep scan (..), array indexing, filters, and recursive descent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-path-query-engine](https://vinkius.com/mcp/json-path-query-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Path Query Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-path-query-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Path Query Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-path-query-engine": {
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

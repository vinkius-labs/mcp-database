# Orama Hybrid Search Query Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/orama-hybrid-search-query-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate syntactically perfect Orama search payloads with deterministic JSON structure.

## Description
The Orama Hybrid Search Query Builder acts as a specialized bridge for AI agents to interact with the Orama search engine. It solves the complex problem of constructing nested, hierarchical JSON payloads required by Orama's 'where' clause syntax. By providing a flat dictionary of filters, this MCP server uses deterministic V8 object mapping to transform simple key-value pairs into precise comparison operators like `eq`, `gt`, and `lt`. This ensures that agents can perform advanced filtering—such as range queries on prices or dates—without the risk of generating invalid syntax. Use `build_orama_query` to generate your payload, `validate_filter_syntax` to check for errors before construction, and `get_operator_mapping_summary` to understand the supported operator tiers.


## Available Tools (3)
- **build_orama_query**: Constructs a nested JSON object for Orama
- **get_operator_mapping_summary**: Returns a summary of Orama operator mapping rules
- **validate_filter_syntax**: Validates the syntax of a filter dictionary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orama Hybrid Search Query Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build an Orama query for 'running shoes' with a price less than 100 and category as 'sports'."

**🤖 AI Agent:**
> { "term": "running shoes", "properties": [], "where": { "price": { "lt": 100 }, "category": { "eq": "sports" } } }

---

**👤 You:**
> "Check if this filter dictionary is valid: {"brand": "Nike", "rating": {"gt": 4}}"

**🤖 AI Agent:**
> The syntax is valid. The filters will be mapped to `eq` for brand and `gt` for rating.

---

**👤 You:**
> "Show me the supported operators in Orama."

**🤖 AI Agent:**
> The supported operators are: `eq`, `gt`, and `lt`.


## ❓ FAQ

**Q: What is the main purpose of this MCP server?**
It automates the creation of complex, nested JSON payloads for Orama search queries, ensuring syntactical correctness using `build_orama_query`.

**Q: How can I ensure my filter dictionary is valid?**
You should use the `validate_filter_syntax` tool to check your dictionary for any unsupported types or invalid characters before attempting to build a query.

**Q: What operators are supported for filtering?**
The server supports `eq` (equality), `gt` (greater than), and `lt` (less than) through its deterministic mapping logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/orama-hybrid-search-query-builder](https://vinkius.com/ai-agent-connect/orama-hybrid-search-query-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orama Hybrid Search Query Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `orama-hybrid-search-query-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orama Hybrid Search Query Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orama-hybrid-search-query-builder": {
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

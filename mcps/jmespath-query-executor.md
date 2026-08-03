# jmespath-query-executor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jmespath-query-executor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deterministic JSON querying using simplified JMESPath syntax.

## Description
The `jmespath-query-executor` provides a reliable way to extract specific data from complex JSON structures. By using a simplified JMESPath syntax, it avoids the risks of executing arbitrary JavaScript. You can use `execute_jmespath_query` to run queries, `validate_query_syntax` to check your query structure, and `inspect_json_schema` to understand your dataset's root level.


## Available Tools (3)
- **execute_jmespath_query**: Executes a JMESPath-like query on JSON data
- **validate_query_syntax**: ", "[]", and "*".

Validates the syntax of a JMESPath-like query string
- **inspect_json_schema**: Analyzes the top-leveled structure of JSON data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **jmespath-query-executor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the name from this JSON: {"user": {"name": "Alice"}} using '.'"

**🤖 AI Agent:**
> "Alice"

---

**👤 You:**
> "Check if this query is valid: 'user.profile.*'"

**🤖 AI Agent:**
> true

---

**👤 You:**
> "What are the top-level keys in this JSON: {"id": 1, "data": []}"

**🤖 AI Agent:**
> ["id", "data"]


## ❓ FAQ

**Q: What tokens are supported in the query string?**
The engine supports three primary tokens: '.' for property access, '[]' for array flattening, and '*' for wildcards.

**Q: How can I verify if my query is valid before running it?**
You can use the `validate_query_syntax` tool to check your string for structural validity.

**Q: Does this tool modify my original JSON data?**
No, the engine treats the input JSON as a read-only structure and builds a new resulting structure without modifying the source.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jmespath-query-executor](https://vinkius.com/mcp/jmespath-query-executor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **jmespath-query-executor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jmespath-query-executor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **jmespath-query-executor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jmespath-query-executor": {
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

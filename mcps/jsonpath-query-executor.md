# JSONPath Query Executor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jsonpath-query-executor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Execute deterministic JSONPath queries against any JSON data.

## Description
The JSONPath Query Executor allows AI agents to navigate and extract specific information from complex, nested JSON structures using a simplified, deterministic syntax. By utilizing tools like `execute_json_path_query`, `validate_path_syntax`, and `get_path_complexity_metrics`, agents can reliably retrieve data without the risks of executing arbitrary JavaScript. This MCP server acts as a bridge, enabling precise data extraction from any JSON payload provided via Vinkius Edge.


## Available Tools (3)
- **execute_jsonpath_query**: Returns the stringified result.

Executes a JSONPath query on provided data
- **get_path_complexity_metrics**: Calculates complexity metrics for a JSONPath string
- **validate_path_syntax**: Validates the syntax of a JSONPath string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSONPath Query Executor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the authors from this JSON: {"store":{"book":[{"author":"Nigel"},{"author":"Errina"}]}} using path $.store.book[*].author"

**🤖 AI Agent:**
> ["Nigel", "Errina"]

---

**👤 You:**
> "Is the path $.store.book[0].title valid?"

**🤖 AI Agent:**
> true

---

**👤 You:**
> "How complex is the path $.store.book[*].author.name?"

**🤖 AI Agent:**
> The path contains 4 segments and includes a wildcard.


## ❓ FAQ

**Q: What kind of JSONPath syntax is supported?**
The engine supports a simplified, deterministic syntax using dot notation for keys and `[*]` wildcards for array iteration.

**Q: How can I check if my query string is valid?**
You can use the `validate_path_syntax` tool to verify your path before execution.

**Q: Is it safe to run queries on large JSON files?**
Yes, the execution is deterministic and uses V8 array methods to ensure predictable behavior and prevent security risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsonpath-query-executor](https://vinkius.com/mcp/jsonpath-query-executor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSONPath Query Executor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jsonpath-query-executor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSONPath Query Executor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jsonpath-query-executor": {
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

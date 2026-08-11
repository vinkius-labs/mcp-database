# JSONPath Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jsonpath-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extract specific values from JSON objects using precise JSONPath expressions.

## Description
JSONPath Extractor provides tools to navigate and select data within complex JSON structures. Use `evaluate_path` to retrieve specific values, `validate_expression_syntax` to verify your path logic, and `get_path_metadata` to inspect the depth and structure of matched elements. It supports standard wildcards, array slicing, and filter expressions for deterministic data retrieval.


## Available Tools (3)
- **evaluate_path**: Performs the primary extraction of data using a provided JSONPath expression
- **get_path_metadata**: Returns information about the structure and complexity of the JSON object relative to a specific path
- **validate_expression_syntax**: Checks if a JSONPath expression is syntactically correct without executing it against data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSONPath Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the name of the first user from this JSON: {"users": [{"name": "Alice"}, {"name": "Bob"}]}"

**🤖 AI Agent:**
> Alice

---

**👤 You:**
> "Get all ages from this JSON: {"people": [{"age": 25}, {"age": 30}, {"age": 35}]}"

**🤖 AI Agent:**
> [25, 30, 35]

---

**👤 You:**
> "Check if the path '$.store.book[0]' is valid for this JSON: {"store": {"book": [{"title": "Example"}]}}"

**🤖 AI Agent:**
> true


## ❓ FAQ

**Q: How do I verify if my JSONPath is correct?**
You can use the `validate_expression_syntax` tool to check the syntax of your expression without needing to provide a JSON object.

**Q: Can I extract multiple values at once?**
Yes, using `evaluate_path` with wildcards or slice notation will return an array of all matching elements found in the JSON object.

**Q: How can I check the nesting level of a specific path?**
The `get_path_metadata` tool provides the depth and whether the path terminates at a leaf node or a container.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsonpath-extractor](https://vinkius.com/mcp/jsonpath-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSONPath Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jsonpath-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSONPath Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jsonpath-extractor": {
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

# URL Query String Deep Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/url-query-string-deep-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Transforms flat URL query strings into deeply nested JSON objects and arrays.

## Description
The URL Query String Deep Parser is a specialized utility designed to bridge the gap between simple key-value pairs and complex data structures. It allows AI agents to interpret hierarchical query parameters using dot notation (e.g., `user.name`) and array notation (e.g., `tags[]`). By utilizing tools like `parse_query_string`, `flatten_to_pairs`, `lookup_deep_value`, and `get_nesting_complexity`, agents can navigate complex API filters and structured URL data with precision.


## Available Tools (4)
- **lookup_deep_value**: g., "user.profile.id"). Returns found value and if access was nested.

Retrieves the value of a specific property located at any depth within the query string
- **parse_query_string**: Returns parsed object, total count, and nested keys count.

Converts a raw query string into its fully structured, nested JSON representation
- **flatten_to_pairs**: Returns array of "key=value" strings.

Extracts all decoded key-value pairs into a simple, flat list for inspection
- **get_nesting_complexity**: Analyzes the structural depth and complexity of the parsed query string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL Query String Deep Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this query string: `name=John&user.id=123&tags[]=dev&tags[]=admin`"

**🤖 AI Agent:**
> { "name": "John", "user": { "id": "123" }, "tags": ["dev", "admin"] }

---

**👤 You:**
> "What is the value of `user.id` in `user.id=456&status=active`?"

**🤖 AI Agent:**
> 456

---

**👤 You:**
> "Check the complexity of `a.b.c=1&d[]=2`."

**🤖 AI Agent:**
> The maximum nesting depth is 3 and arrays are present in the structure.


## ❓ FAQ

**Q: How does the parser handle nested objects?**
The parser uses dot notation to identify hierarchy. For example, a key like `user.profile.id` will result in a nested JSON structure: `{ "user": { "profile": { "id": "..." } } }`.

**Q: Can it detect arrays in the query string?**
Yes, any key ending with `[]` is automatically treated as an array. The `get_nesting_complexity` tool can specifically report if arrays are present in your string.

**Q: Does it support URI decoding?**
Yes, all keys and values are processed through standard URI decoding to ensure characters like `%20` are correctly converted back to spaces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/url-query-string-deep-parser](https://vinkius.com/mcp/url-query-string-deep-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL Query String Deep Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `url-query-string-deep-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL Query String Deep Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-query-string-deep-parser": {
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

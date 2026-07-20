# OpenAPI Context Window Packer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openapi-context-window-packer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Prune massive OpenAPI specs to fit within LLM context windows.

## Description
The OpenAPI Context Window Packer is a precision engine designed to compress large OpenAPI/Swagger specifications. It solves the problem of AI agents failing to use tools because the API spec exceeds their token limit. By using `compress_openapi_spec`, you can prune paths not in your target list and strip unused components via dependency tracing. You can also use `analyze_endpoint_coverage` to verify presence and `trace_schema_dependencies` to identify required schemas.


## Available Tools (3)
- **compress_openapi_spec**: Compresses OpenAPI spec
- **analyze_endpoint_coverage**: Analyzes endpoint coverage
- **trace_schema_dependencies**: Traces schema dependencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAPI Context Window Packer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my target endpoints are present in this spec."

**🤖 AI Agent:**
> The `analyze_endpoint_coverage` tool reports that 3 out of 5 target endpoints were found in the provided specification.

---

**👤 You:**
> "Compress this large OpenAPI spec to fit a 2000 token budget."

**🤖 AI Agent:**
> The specification has been compressed. The original size was estimated at 15,000 tokens, and the packed version is now approximately 1,850 tokens.

---

**👤 You:**
> "Which schemas are needed for the /users endpoint?"

**🤖 AI Agent:**
> The `trace_schema_dependencies` tool identified that the `/users` endpoint requires the `User`, `Address`, and `Role` schemas.


## ❓ FAQ

**Q: How does the compression work?**
The engine uses deterministic pruning. It removes all paths not in your `targetEndpoints` and then traces `$ref` pointers to remove any schemas that are no longer reachable, ensuring the resulting spec is structurally valid.

**Q: Will my API specification break after compression?**
No. The tool ensures schema integrity by performing a graph traversal. Any component or schema required by your target endpoints is strictly preserved.

**Q: Can I control the size of the output?**
Yes. Using `compress_openapi_spec`, you can set a `maxTokenBudget`. The engine will iteratively truncate description fields until the specification fits within your specified budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openapi-context-window-packer](https://vinkius.com/mcp/openapi-context-window-packer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenAPI Context Window Packer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openapi-context-window-packer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenAPI Context Window Packer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openapi-context-window-packer": {
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

# API Pagination Logic Verifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-pagination-logic-verifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Audit API endpoints for correct pagination patterns to prevent memory exhaustion.

## Description
The API Pagination Logic Verifier is an AST-based engine designed to identify 'unbounded' API endpoints. By parsing source code, it detects if implementations correctly use offset/limit or cursor-based pagination and enforces maximum limits to prevent service crashes caused by memory exhaustion. Use `analyze_offset_pagination` to check parameter structures, `verify_limit_enforcement` to audit guardrails, and `inspect_pagination_metadata` to ensure response objects include necessary navigation pointers.


## Available Tools (3)
- **inspect_pagination_metadata**: Verifies that the API response structure includes the necessary information for clients to navigate pages
- **verify_limit_enforcement**: Audits whether the code implements a guardrail to prevent excessively large requests
- **analyze_offset_pagination**: Checks if an endpoint implementation correctly accepts and structures parameters for offset/limit pagination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API Pagination Logic Verifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this handler uses pagination: `const { limit, offset } = req.query;`"

**🤖 AI Agent:**
> The tool identified both `limit` and `offset` parameters in the destructuring pattern.

---

**👤 You:**
> "Does this code enforce a maximum limit of 50? `if (limit > 50) limit = 50;`"

**🤖 AI Agent:**
> Yes, the logic correctly compares the incoming limit against the threshold of 50.

---

**👤 You:**
> "Verify if the response contains metadata: `res.json({ totalCount: 100, nextCursor: 'abc' });`"

**🤖 AI Agent:**
> The response structure is valid and includes both `totalCount` and a navigation pointer.


## ❓ FAQ

**Q: How does the verifier detect pagination errors?**
The engine uses Abstract Syntax Tree (AST) parsing to analyze code structure without execution, looking for specific patterns in variable declarations and function parameters.

**Q: Can I use this to check for cursor-based pagination?**
Yes, by using `inspect_pagination_metadata`, you can verify if the response object includes navigation pointers like `nextCursor`.

**Q: What happens if a limit is not enforced?**
If `verify_limit_enforcement` detects that an incoming limit can bypass the threshold, it will flag a violation, indicating a risk of memory exhaustion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-pagination-logic-verifier](https://vinkius.com/mcp/api-pagination-logic-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **API Pagination Logic Verifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `api-pagination-logic-verifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **API Pagination Logic Verifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "api-pagination-logic-verifier": {
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

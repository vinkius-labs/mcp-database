# HTTP Status Reference Lookup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/http-status-reference-lookup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [networking](../categories/networking.md)

Retrieve official names, RFC references, and semantic properties for HTTP status codes.

## Description
The HTTP Status Reference Lookup MCP server provides a deep dive into the semantics of HTTP response codes. It allows you to query specific details for any status code, including its official name, RFC reference, and whether it is cacheable or retryable. You can use `get_status_metadata` to retrieve technical definitions, `list_codes_by_category` to browse ranges like 2xx or 4xx, and `check_scenario_consistency` to validate if a status code matches your payload's content, helping prevent semantic mismatches in API responses.

### Available Tools

`lookup_status`, `list_all_statuses`, `validate_status_scenario`


## Available Tools (3)
- **list_all_statuses**: List all registered HTTP status codes
- **lookup_status**: Look up details for a specific HTTP status and its semantics
- **validate_status_scenario**: Validate if an HTTP status code is appropriate for a given response scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTTP Status Reference Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the details for HTTP status code 404?"

**🤖 AI Agent:**
> HTTP 404 Not Found: The server cannot find the requested resource. It belongs to the Client Error category.

---

**👤 You:**
> "Is it okay to return a 200 OK when the response body contains an error message?"

**🤖 AI Agent:**
> No, that is considered a semantic mismatch. The status code and payload are inconsistent.

---

**👤 You:**
> "List all the HTTP status codes available in this server."

**🤖 AI Agent:**
> The server contains a registry of all standard HTTP status codes from 100 to 599.


## ❓ FAQ

**Q: What can I do with this MCP server?**
You can use it to look up technical details for any HTTP status code, list all known codes, or validate if a specific response scenario is semantically correct using `check_scenario_consistency`. Tools available: `lookup_status`, `list_all_statuses`, `validate_status_scenario`.

**Q: How do I check if a 200 OK response with an error body is valid?**
You can use the `check_scenario_consistency` tool by providing the status code 200 and setting `isErrorBody` to true. It will flag this as an inconsistency.

**Q: Does it support all HTTP status codes?**
It supports the standard registry of HTTP status codes, including 1xx, 2xx, 3xx, 4xx, and 5xx ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/http-status-reference-lookup](https://vinkius.com/mcp/http-status-reference-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTTP Status Reference Lookup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `http-status-reference-lookup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTTP Status Reference Lookup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "http-status-reference-lookup": {
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

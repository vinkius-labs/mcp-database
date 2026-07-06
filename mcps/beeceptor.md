# Beeceptor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beeceptor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Mock APIs, intercept requests, and manage proxy rules directly from your AI agent.

## Description
Connect **Beeceptor** to your AI agent to build, manage, and monitor mock APIs and HTTP proxies through natural language.

### What you can do

- **Endpoint Management** — Configure CORS, request logging, and authentication for your subdomains using `update_settings`.
- **Mock Rules** — Create, update, and reorder rules via `create_rule` and `reorder_rules` to simulate complex API behaviors.
- **Request Inspection** — List and inspect incoming HTTP requests in real-time with `list_requests` to debug webhooks or integrations.
- **API Specifications** — Upload OpenAPI or Swagger specs using `upload_spec` to automatically generate mock endpoints.
- **State Management** — Maintain state across mock calls using key-value storage tools like `upsert_state` and `get_state_item`.

### How it works

1. Subscribe to this server
2. Enter your Beeceptor API Key
3. Start mocking and debugging APIs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly mock backend dependencies without writing server code.
- **QA Engineers** — simulate edge cases, timeouts, and error responses to test application resilience.
- **Backend Developers** — debug webhooks and third-party callbacks by inspecting payloads in real-time.


## Available Tools (29)
- **delete_state**: Delete state items (Bulk)
- **list_state**: Get all state
- **add_certificate**: Add mTLS certificate
- **bulk_replace_rules**: Bulk replace mock rules
- **create_rule**: Create mock rule
- **delete_all_rules**: Delete all mock rules
- **delete_certificate**: Delete mTLS certificate
- **delete_request**: Delete single request
- **delete_requests**: Delete request history
- **delete_rule**: Delete mock rule
- **delete_spec**: Delete specification
- **delete_state_item**: Delete single state item
- **download_multipart**: Download multipart file
- **get_job_status**: Get spec upload job status
- **get_request**: Get single request
- **get_rule**: Get single mock rule
- **get_settings**: Get endpoint settings
- **get_spec_details**: Get specification details
- **get_state_item**: Get single state item
- **list_certificates**: List mTLS certificates
- **list_requests**: Get request history
- **list_rules**: Get all mock rules
- **reorder_rules**: Reorder mock rules
- **update_rule_full**: Update mock rule (Full)
- **update_rule_partial**: Update mock rule (Partial)
- **update_settings**: Update endpoint settings
- **upload_blob**: Upload binary blob
- **upload_spec**: Upload API specification
- **upsert_state**: Upsert state (Bulk)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beeceptor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mock rules for the 'payment-api' endpoint."

**🤖 AI Agent:**
> I've retrieved the rules for 'payment-api'. You have 3 active rules: 1. GET /success (200 OK), 2. POST /authorize (401 Unauthorized), and 3. GET /balance (200 OK).

---

**👤 You:**
> "Show me the last 5 requests received at 'my-webhook-test'."

**🤖 AI Agent:**
> Fetching recent traffic... I found 5 requests. The most recent one was a POST to /callback with a JSON payload containing 'event: user_signup'. Would you like to see the full headers for this request?

---

**👤 You:**
> "Enable CORS and request logging for the 'dev-sandbox' endpoint."

**🤖 AI Agent:**
> Settings updated successfully for 'dev-sandbox'. CORS is now enabled and request logging is active.


## ❓ FAQ

**Q: Can I enable CORS for my mock endpoint through the AI?**
Yes. You can use the `update_settings` tool to toggle CORS, request logging, and other endpoint features instantly.

**Q: How do I see the payloads of recent requests sent to my Beeceptor subdomain?**
Use the `list_requests` tool. It retrieves a list of recent incoming HTTP calls, allowing your agent to analyze headers and body content.

**Q: Is it possible to simulate a database or state between API calls?**
Yes, Beeceptor provides a key-value store. You can use `upsert_state` to save data and `get_state_item` to retrieve it in subsequent mock responses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beeceptor](https://vinkius.com/mcp/beeceptor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beeceptor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beeceptor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beeceptor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beeceptor": {
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

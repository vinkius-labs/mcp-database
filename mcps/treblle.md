# Treblle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/treblle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor, document, and analyze your API traffic in real-time. Ingest request and response data directly into Treblle for instant observability.

## Description
Connect your **Treblle** account to your AI agent to streamline API monitoring and observability. This server allows you to send API traffic data directly to Treblle, helping you maintain high-quality documentation and security standards.

### What you can do

- **API Ingestion** — Send full request and response payloads to your Treblle dashboard using the `ingest_api_data` tool.
- **Observability** — Monitor API performance and errors in real-time as your agent processes or simulates traffic.
- **Automatic Masking** — Ensure security with Treblle's built-in masking for sensitive fields like passwords and credit card numbers.
- **Custom Metadata** — Attach trace IDs, user IDs, or environment identifiers to your ingested data for better filtering.

### How it works

1. Subscribe to this server
2. Enter your Treblle API Key and SDK Token
3. Start ingesting API data directly from your conversation or automated workflows

### Who is this for?

- **Backend Developers** — quickly log and debug API interactions without manual instrumentation
- **DevOps Engineers** — monitor API health and traffic patterns directly from the terminal or AI assistant
- **QA Engineers** — capture and report API errors with full context during testing phases


## Available Tools (1)
- **ingest_api_data**: Sensitive fields (passwords, CCs, SSNs) are automatically masked before transmission.

Send API request/response data to Treblle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Treblle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ingest this API request and response data into Treblle: { "server": { ... }, "request": { ... }, "response": { ... } }"

**🤖 AI Agent:**
> I've successfully ingested the API data into Treblle. You can now view the request details, performance metrics, and documentation in your Treblle dashboard.

---

**👤 You:**
> "Send this API error payload to Treblle with metadata trace-id 'abc-123'."

**🤖 AI Agent:**
> The error payload has been sent to Treblle and tagged with trace-id 'abc-123'. It will appear in your error logs for further investigation.

---

**👤 You:**
> "Log a successful GET request to /users into Treblle using the ingest_api_data tool."

**🤖 AI Agent:**
> I've logged the GET /users request to Treblle. The traffic data has been processed and is now available for monitoring.


## ❓ FAQ

**Q: How do I send API traffic data to my Treblle dashboard?**
Use the `ingest_api_data` tool. You need to provide the JSON payload containing the server, request, and response information as defined in the Treblle schema.

**Q: Is my sensitive data like passwords or credit cards safe when ingesting?**
Yes. Treblle automatically masks sensitive fields (passwords, CCs, SSNs) before the data is transmitted and stored, ensuring compliance and security.

**Q: Can I add custom identifiers like a trace-id to the ingested data?**
Absolutely. You can use the optional `metadata` parameter in the `ingest_api_data` tool to include flat key-value pairs like `trace-id`, `user-id`, or `env-id`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/treblle](https://vinkius.com/mcp/treblle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Treblle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `treblle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Treblle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "treblle": {
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

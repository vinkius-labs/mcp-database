# Loggly (Cloud Log Management API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loggly-cloud-log-management-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Manage cloud logs via Loggly — send events, execute Lucene searches, and analyze infrastructure metrics directly from your AI agent.

## Description
Connect your **Loggly** account to any AI agent to streamline your observability and debugging workflows. This MCP server allows you to interact with your logs using natural language, making it easier to find errors, monitor performance, and manage your logging infrastructure.

### What you can do

- **Log Ingestion** — Send single or bulk log events (plaintext or JSON) directly to Loggly for real-time indexing.
- **Advanced Search** — Execute complex queries using Lucene syntax to filter through millions of events across specific timeframes.
- **Result Retrieval** — Fetch paginated search results using Result Set IDs (rsid) for deep analysis of system behavior.
- **Field Analysis & Faceting** — List available log fields and get value counts (faceting) to understand data distribution and common errors.
- **Account Management** — Retrieve customer info, subscription limits, and list active users and roles within your Loggly organization.

### How it works

1. Subscribe to this server
2. Provide your Loggly Subdomain, API Token, and Customer Token
3. Start querying and sending logs from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to correlate logs. Your AI can now act as a proactive SRE or DevOps engineer, identifying patterns and troubleshooting issues in seconds.

### Who is this for?

- **DevOps & SREs** — Quickly search for production errors and analyze log trends without leaving the terminal or chat interface.
- **Backend Developers** — Send debug events during development and verify log ingestion in real-time.
- **Security Analysts** — Audit user roles and search for suspicious patterns using structured log queries.


## Available Tools
- **get_customer_info**: Retrieve Loggly account details
- **get_events**: Max 5,000 events per search.

Retrieve events for a given search rsid
- **get_field_values**: Get counts of values for a specific field (Faceting)
- **list_fields**: List available fields in Loggly
- **list_users**: Retrieve a list of active users
- **search_events**: Use get_events with the rsid to fetch the actual logs.

Initiate an asynchronous search query
- **send_bulk_events**: The events_data must be line-separated (up to 5MB per batch).

Send batches of line-separated events to Loggly
- **send_event**: Use is_json=true if event_data is a JSON string. Max size 1MB.

Send a single or multiline event to Loggly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loggly (Cloud Log Management API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all logs containing 'error' in the last 4 hours."

**🤖 AI Agent:**
> I've initiated a search for 'error' from the last 4 hours. The Result Set ID is `123456789`. I'll now fetch the events for you...

---

**👤 You:**
> "Send a JSON log event with tag 'production' saying {'status': 'ok', 'service': 'api'}."

**🤖 AI Agent:**
> Successfully sent the JSON event to Loggly with the 'production' tag. The response was 'ok'.

---

**👤 You:**
> "List all active users and their roles in my Loggly account."

**🤖 AI Agent:**
> I've retrieved the user list. You have 3 active users: 'admin_user' (Role: Administrator), 'dev_user' (Role: User), and 'audit_bot' (Role: Read-Only).


## ❓ FAQ

**Q: How do I search for logs and see the results?**
Searching is a two-step process: first, use `search_events` with your Lucene query to get a Result Set ID (rsid). Then, use `get_events` with that rsid to retrieve the actual log data.

**Q: Can I send JSON logs directly from the AI?**
Yes! Use the `send_event` tool and set `is_json` to true. You can pass a JSON string in the `event_data` field, and Loggly will parse it as a structured object.

**Q: How can I see which fields are most common in my logs?**
You can use `list_fields` to see all available fields, or use `get_field_values` with a specific field name to get a count of the top values (faceting) for that field.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loggly-cloud-log-management-api](https://vinkius.com/mcp/loggly-cloud-log-management-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loggly (Cloud Log Management API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `loggly-cloud-log-management-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loggly (Cloud Log Management API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loggly-cloud-log-management-api": {
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

# Svix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/svix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your webhook infrastructure via Svix — orchestrate applications, configure endpoints, and monitor message delivery directly from any AI agent.

## Description
Connect your **Svix** account to any AI agent and take full control of your webhook lifecycle through natural conversation.

### What you can do

- **Application Management** — List, create, and update applications to group your endpoints and messages logically.
- **Endpoint Configuration** — Create and manage destination URLs, set event filters, and enable or disable specific endpoints for your apps.
- **Message Delivery** — Create and track messages, inspect payloads, and retrieve detailed delivery status for every event.
- **Debugging & Monitoring** — List message and endpoint attempts to identify failures and ensure your integrations are running smoothly.
- **Lifecycle Control** — Delete stale applications or endpoints and update configurations instantly without touching the dashboard.

### How it works

1. Subscribe to this server
2. Enter your Svix API Secret Key
3. Start managing your webhooks from Claude, Cursor, or any MCP-compatible client

No more manual debugging through logs. Your AI acts as a dedicated DevOps engineer for your event-driven architecture.

### Who is this for?

- **Backend Engineers** — quickly configure new webhook destinations and test event delivery without leaving the IDE.
- **DevOps Teams** — monitor delivery attempts and troubleshoot failing endpoints using natural language queries.
- **Product Integrations Leads** — manage customer-facing webhook applications and verify message flows in real-time.


## Available Tools (15)
- **create_application**: Create a new Svix application
- **delete_application**: Delete a Svix application
- **create_endpoint**: Create a new endpoint for a Svix application
- **create_message**: Send a new webhook message
- **delete_endpoint**: Delete a Svix endpoint
- **get_application**: Get details of a specific Svix application
- **get_endpoint**: Get details of a specific Svix endpoint
- **get_message**: Get details of a specific Svix message
- **list_applications**: List Svix applications
- **list_endpoint_attempts**: List delivery attempts for a specific endpoint
- **list_endpoints**: List endpoints for a Svix application
- **list_message_attempts**: List delivery attempts for a specific message
- **list_messages**: List messages sent for a Svix application
- **update_application**: Update an existing Svix application
- **update_endpoint**: Update an existing Svix endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Svix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Svix applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 2 active apps: 'Main API' (ID: app_2X...) and 'Billing Service' (ID: app_9Y...). Which one would you like to inspect?

---

**👤 You:**
> "Create a new endpoint for app_2X... with URL https://webhook.site/test and subscribe to 'user.created' events."

**🤖 AI Agent:**
> Endpoint created successfully! The new endpoint ID is ep_3Z... and it is now configured to receive 'user.created' events at the specified URL.

---

**👤 You:**
> "Show me the details for message msg_4W..."

**🤖 AI Agent:**
> Fetching message details... Message msg_4W... was sent with event type 'invoice.paid'. It has been successfully delivered to 1 endpoint and is currently pending on another.


## ❓ FAQ

**Q: How can I see all my current Svix applications?**
Simply ask the agent to run the `list_applications` tool. It will return a complete list of applications in your Svix workspace along with their IDs and names.

**Q: Can I check why a specific webhook message failed to deliver?**
Yes! Use the `list_message_attempts` tool with the message ID. Your agent will fetch the history of delivery attempts, including response codes and timestamps for debugging.

**Q: Is it possible to temporarily stop sending webhooks to a specific URL?**
Yes. You can use the `update_endpoint` tool and set the `disabled` parameter to `true` for that specific endpoint ID. This will pause delivery without deleting the configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/svix](https://vinkius.com/mcp/svix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Svix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `svix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Svix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "svix": {
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

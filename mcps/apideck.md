# Apideck MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apideck)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Unify your software stack with Apideck — manage CRM contacts, orchestrate Vault connections, and execute proxy requests across dozens of platforms through one API.

## Description
Connect **Apideck** to your AI agent to streamline how you interact with multiple SaaS platforms. By using Apideck's Unified APIs, your agent can communicate with various CRM providers and manage user integrations without writing custom code for every service.

### What you can do

- **Unified CRM Access** — List and filter contacts across different CRM providers like Salesforce, HubSpot, or Pipedrive using the `list_crm_contacts` tool.
- **Vault Management** — Create sessions for users to link their own accounts (`create_vault_session`), list existing connections, and retrieve or delete specific service links.
- **API Proxying** — Execute direct requests to downstream service endpoints using `execute_proxy` when you need specific functionality not covered by the unified schema.
- **Connection Auditing** — Inspect the status and details of active integrations using `get_vault_connection` to ensure data flow is healthy.

### How it works

1. Subscribe to this server
2. Provide your Apideck API Key, App ID, and Consumer ID
3. Start querying your unified ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — who want to interact with multiple APIs through a single, normalized interface directly from their IDE.
- **Product Managers** — who need to audit user connections and CRM data across different environments without manual API calls.
- **Support Teams** — who need to verify if a customer's integration is correctly configured in the Vault through natural language.


## Available Tools (6)
- **list_crm_contacts**: g., salesforce, hubspot) using the Unified CRM API.

List CRM contacts from a unified integration
- **delete_vault_connection**: Delete a Vault connection
- **get_vault_connection**: Get a specific Vault connection
- **execute_proxy**: Execute a Proxy API request
- **list_vault_connections**: List Vault connections
- **create_vault_session**: Create a Vault session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apideck** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all CRM contacts from the hubspot integration."

**🤖 AI Agent:**
> I've retrieved the contacts from HubSpot. I found 12 contacts, including 'Alice Smith' (alice@example.com) and 'Bob Jones' (bob@example.com). Would you like more details on any of them?

---

**👤 You:**
> "Show me all active Vault connections for the current consumer."

**🤖 AI Agent:**
> You currently have 3 active connections in the Vault: 'salesforce', 'hubspot', and 'slack'. All connections are reported as healthy.

---

**👤 You:**
> "Create a Vault session with a redirect URI to https://example.com/dashboard."

**🤖 AI Agent:**
> I've created a new Vault session. You can direct the user to this URL to manage their integrations: https://vault.apideck.com/session/example-token


## ❓ FAQ

**Q: Can I fetch contacts from a specific CRM like Salesforce or HubSpot?**
Yes. Use the `list_crm_contacts` tool and provide the `service_id` (e.g., 'salesforce') to retrieve unified contact data from that specific integration.

**Q: How do I allow my users to configure their own integrations?**
You can use the `create_vault_session` tool to generate a secure session URL where users can manage their connections within the Apideck Vault.

**Q: What if I need to call an API endpoint that isn't part of the unified schema?**
The `execute_proxy` tool allows you to make direct calls to any downstream service URL using the stored credentials for a specific `service_id`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apideck](https://vinkius.com/mcp/apideck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apideck** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apideck` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apideck** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apideck": {
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

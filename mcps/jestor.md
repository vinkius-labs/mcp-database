# Jestor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jestor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage data, workflows, and records via Jestor low-code API.

## Description
Empower your AI agents with Jestor's low-code internal tools platform. This MCP server allows you to list objects (tables), retrieve and list records, manage users, and monitor workflows and dashboards directly through the Jestor API. Ideal for automating internal operations and database management.


## Available Tools (10)
- **get_me**: Use this to verify connection status and current permissions.

Gets current authenticated user info
- **get_object**: Useful for understanding field types and relationships within a specific table.

Retrieves details/schema for a specific object
- **get_record**: Essential for deep-diving into a specific entry in the database.

Retrieves details for a specific record
- **list_apps**: Useful for discovering high-level toolsets available to the user.

Lists all installed internal apps
- **list_dashboards**: Use this to identify where aggregated data visualizations are located.

Lists all configured dashboards
- **list_objects**: Returns object names and labels. Use this to discover available datasets before querying specific records.

Lists all objects (tables) in your Jestor account
- **list_records**: This is the primary tool for browsing data within a table (e.g., listing all "Tasks" or "Clients").

Lists records for a specific object
- **list_users**: Returns names, emails, and IDs. Useful for identifying record owners or system administrators.

Lists all users in the organization
- **list_webhooks**: Use this to audit third-party integrations.

Lists all configured webhooks
- **list_workflows**: Useful for auditing system logic and event-driven actions.

Lists all automated workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jestor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all objects in my Jestor account."

**🤖 AI Agent:**
> I'll fetch the list of all tables and objects for you.

---

**👤 You:**
> "Show me the records for the 'Invoices' object."

**🤖 AI Agent:**
> I'll retrieve the records from your Invoices table in Jestor.

---

**👤 You:**
> "Check the status of my workflows."

**🤖 AI Agent:**
> I'll look up the list of configured workflows and their status in Jestor.


## ❓ FAQ

**Q: How do I get Jestor API credentials?**
Log in to your Jestor account, navigate to Lowcode > API & Tokens, and generate a new token.

**Q: What are 'objects' in Jestor?**
Objects are similar to tables in a database. They store your data and records.

**Q: Can I see my workflows?**
Yes, the list_workflows tool provides a list of all active automations in your Jestor account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jestor](https://vinkius.com/mcp/jestor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jestor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jestor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jestor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jestor": {
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

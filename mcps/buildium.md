# Buildium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buildium)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage rental properties via Buildium — track units, tenants, and maintenance tasks directly from any AI agent.

## Description
Connect your **Buildium** account to any AI agent and orchestrate your property management, tenant relations, and maintenance workflows through natural conversation.

### What you can do

- **Property Oversight** — List and retrieve detailed metadata for all rental properties and individual units in your portfolio.
- **Tenant Management** — List all tenants and retrieve detailed profiles, including lease information and balances.
- **Maintenance Tracking** — Query and monitor tasks and work orders to ensure timely property upkeep.
- **Vendor Coordination** — Access your directory of vendors and internal staff managed within the platform.
- **Company Insights** — Retrieve core company information and settings straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Buildium Client ID and Client Secret
3. Start managing your property portfolio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Managers** — quickly check unit availability or tenant balances without manual dashboard searches.
- **Leasing Agents** — retrieve property and unit details straight from their communication tools.
- **Maintenance Coordinators** — monitor work orders and vendor lists using natural language.


## Available Tools (10)
- **get_company_info**: Retrieve core company information
- **get_property**: Get details of a specific property
- **get_tenant**: Get details of a specific tenant
- **get_unit**: Get details of a specific unit
- **list_properties**: List all rental properties
- **list_tasks**: List all maintenance tasks
- **list_tenants**: List all rental tenants
- **list_units**: List all rental units
- **list_vendors**: List all vendors
- **list_work_orders**: List all work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buildium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my rental properties in Buildium."

**🤖 AI Agent:**
> I've retrieved your properties. You have 3 properties in your portfolio: 'Evergreen Terrace' (ID: prop_1), 'Maple Street Apartments' (ID: prop_2), and 'Oak Lane' (ID: prop_3).

---

**👤 You:**
> "Show the balance for tenant John Doe (ID 123)."

**🤖 AI Agent:**
> John Doe currently has a total balance of $1,250.00 due. His lease is active until December 31st, 2026.

---

**👤 You:**
> "List the recent maintenance work orders."

**🤖 AI Agent:**
> Retrieving work orders... There are 5 recent orders, including 'Fix Leaky Faucet' (Status: In Progress) and 'Repaint Unit 4B' (Status: New).


## ❓ FAQ

**Q: Can I check the balance for a specific tenant using the agent?**
Yes! Use the `get_tenant` tool with the Tenant ID. Your agent will fetch the detailed profile, including the current total balance due.

**Q: How do I list all the active maintenance tasks?**
Simply ask the agent to `list_tasks`. It will retrieve the current maintenance tasks from your Buildium account, including descriptions and status information.

**Q: Does the integration allow creating a new work order?**
The current toolset focuses on querying and monitoring (Read-Only) for operational efficiency. Creating or updating work orders should be managed via the Buildium administrator portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buildium](https://vinkius.com/mcp/buildium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buildium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buildium` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buildium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buildium": {
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

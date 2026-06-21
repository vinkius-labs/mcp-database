# Rentvine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rentvine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage your property portfolio via Rentvine — list properties, manage units, and track leases directly from any AI agent.

## Description
Connect your **Rentvine** account to any AI agent and take full control of your property management workflows through natural conversation.

### What you can do

- **Property Management** — List all property records, including single-family homes and multi-unit complexes, or fetch specific details by ID.
- **Unit Tracking** — Manage individual rental units within your properties, including creating new units or retrieving specific unit metadata.
- **Lease Administration** — Query all tenant lease agreements, terms, and statuses to stay on top of your rental operations.
- **Data Updates** — Update property details or lease terms directly through the agent to keep your records synchronized.
- **Deep Data Sideloading** — Use the include parameter to fetch related resources like tenants or property details in a single request.

### How it works

1. Subscribe to this server
2. Enter your Rentvine API Token
3. Start managing your real estate portfolio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Managers** — instantly retrieve property statuses, unit availability, and lease terms without navigating the Rentvine dashboard.
- **Real Estate Operations** — automate the retrieval of property data for reporting or tenant communication.
- **Asset Managers** — check portfolio health and lease statuses straight from your AI assistant.


## Available Tools (20)
- **create_lease**: Create a new lease
- **create_property**: Create a new property
- **create_tenant**: Create a new tenant record
- **create_unit**: Add a unit to a property
- **create_work_order**: Create a new maintenance request
- **get_lease**: Retrieve lease details
- **get_property**: Retrieve a specific property
- **get_tenant**: Retrieve tenant details
- **get_unit**: Retrieve unit details
- **get_work_order**: Retrieve work order details
- **list_charges**: List charges
- **list_journal_entries**: Retrieve accounting records
- **list_leases**: List all leases
- **list_payments**: List payments received
- **list_properties**: List all properties
- **list_tenants**: List all tenants
- **list_units**: List all units
- **list_work_orders**: List all work orders
- **update_lease**: Update lease terms or status
- **update_property**: Update property details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rentvine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all properties in my Rentvine account."

**🤖 AI Agent:**
> I've retrieved your property list. You have 12 active properties, including 'Sunset Apartments' (ID: prop_123) and 'Oak Street Home' (ID: prop_456). Would you like to see details for a specific one?

---

**👤 You:**
> "Show me the details for unit ID unit_789."

**🤖 AI Agent:**
> Fetching unit details... Unit 789 is a 2-bedroom apartment located in 'Sunset Apartments'. It is currently listed as 'Vacant' with a monthly rent of $1,500.

---

**👤 You:**
> "Update the lease ID lease_555 status to 'Renewed'."

**🤖 AI Agent:**
> Processing update... The lease agreement lease_555 has been successfully updated to 'Renewed'. All associated records have been synchronized.


## ❓ FAQ

**Q: Can I retrieve the full details of a specific property by its ID?**
Yes! Use the `get_property` tool with the specific Property ID. You can also use the `include` parameter to sideload related data like units or tenants in the same response.

**Q: How do I get a list of all current lease agreements?**
Simply ask the agent to run the `list_leases` tool. It will return a list of lease agreements, including their terms, statuses, and associated IDs for further inspection.

**Q: Can I add a new unit to an existing property through the AI?**
Yes, you can use the `create_unit` tool. Provide the necessary unit data in the payload, and the agent will create the new rental unit record within your Rentvine account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rentvine](https://vinkius.com/mcp/rentvine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rentvine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rentvine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rentvine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rentvine": {
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

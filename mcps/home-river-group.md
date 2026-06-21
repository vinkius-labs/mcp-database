# Home River Group MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/home-river-group)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Connect and manage Home River Group properties, units, and residents via Entrata API.

## Description
Empower your AI agents to interact with Home River Group's property management system. This MCP server allows listing properties, checking unit availability, managing resident information, tracking work orders, and creating leads directly through Entrata. Perfect for automating property maintenance workflows and prospect management.


## Available Tools
- **create_lead**: Submits a new lead/prospect to Home River Group
- **create_work_order**: Creates a new maintenance work order
- **get_availability**: Checks availability for units in a property
- **get_leads**: Lists sales leads and prospects
- **get_lease_info**: Retrieves detailed lease information for residents
- **get_ledgers**: Retrieves financial ledgers for residents
- **get_properties**: This is the starting point to get PropertyIDs needed for other tools. You can filter by specific property IDs or search by name in the results.

Lists properties managed by Home River Group
- **get_residents**: You can filter by propertyId to see residents of a specific building.

Lists residents across properties
- **get_units**: Requires a valid PropertyID.

Lists units for a specific property ID
- **get_work_orders**: Filtering by propertyId is highly recommended.

Lists maintenance work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home River Group** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all properties managed by Home River Group."

**🤖 AI Agent:**
> I'll fetch the list of properties for you.

---

**👤 You:**
> "Check for any open maintenance requests for property ID 123."

**🤖 AI Agent:**
> I'll check the current work orders for that property.

---

**👤 You:**
> "Find all units available for lease in building 456."

**🤖 AI Agent:**
> I'll retrieve the current unit availability for you.


## ❓ FAQ

**Q: How do I get API credentials for Home River Group?**
You need to log in to your Entrata instance (homeriver.entrata.com) and navigate to Setup > Company > API Access. If you don't have access, contact your system administrator.

**Q: Can I create work orders with this MCP?**
Yes, you can use the create_work_order tool to submit new maintenance requests directly into the system.

**Q: Is the subdomain required?**
It defaults to 'homeriver'. If your specific instance uses a different subdomain, you should provide it during setup.

**Q: Are these real-time updates?**
Yes, all data retrieved and created is processed directly through the Entrata API in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/home-river-group](https://vinkius.com/mcp/home-river-group)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home River Group** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `home-river-group` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home River Group** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-river-group": {
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

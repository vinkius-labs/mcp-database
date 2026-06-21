# Fivetran MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fivetran)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage data movement via Fivetran — monitor connectors and destinations, handle groups, track sync states, and audit users directly from any AI agent.

## Description
Connect your **Fivetran** account to any AI agent and take full control of your automated data movement and ELT pipelines through natural conversation.

### What you can do

- **Connector Orchestration** — List all connectors within specific groups and retrieve detailed configuration, synced schema details, and setup states natively
- **Destination Auditing** — Retrieve configuration details for destination databases or data warehouses connected to your groups to verify delivery boundaries
- **Group Management** — List all groups (destinations) created in your Fivetran account and extract identifiers and creation metadata limitlessly
- **Sync State Monitoring** — Identify precise active sync statuses and validate physical data movement progress across your organizational pipelines securely
- **User & Team Oversight** — Enumerate all registered users and RBAC teams in the workspace to monitor access levels and administrative status flawlessy
- **Pipeline Discovery** — Analyze specific localized variables decoding active data routes and extracting hidden structural constraints within your ELT flows
- **Resource Mapping** — Retrieve complex structural arrays defining precisely which sources are mapped to which destinations globally across your account

### How it works

1. Subscribe to this server
2. Enter your Fivetran API Key and API Secret (found in Account Settings > API Config)
3. Start managing your data movement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor sync states and verify connector configurations without opening the Fivetran UI
- **Analytics Leads** — audit data pipelines and verify destination settings using natural language
- **IT Admins** — monitor user access and workspace team structures in real-time through natural conversation
- **Developers** — test and debug data integration parameters and verify schema mappings through the chat interface


## Available Tools
- **list_connectors**: List connectors in group
- **get_connector**: Get connector details
- **list_groups**: List all groups
- **get_group**: Get group details
- **get_destination**: Get destination for group
- **list_users**: List all users
- **list_teams**: List all teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fivetran** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Fivetran groups in my account"

**🤖 AI Agent:**
> Retrieving groups... I found 3 groups (destinations): 'Marketing-Analytics', 'Product-Insights', and 'Finance-Sync'. Which one would you like to see the connectors for?

---

**👤 You:**
> "What is the status of connector 'conn_abc123'?"

**🤖 AI Agent:**
> Retrieving connector details... Connector 'conn_abc123' (PostgreSQL) is currently 'Active'. The last sync finished 15 minutes ago with no errors. The next sync is scheduled for top of the hour.

---

**👤 You:**
> "List all users in the Fivetran workspace"

**🤖 AI Agent:**
> Retrieving users... I found 5 registered users. Highlights include 'Admin User' (Account Administrator), 'Data Analyst' (Analyst), and 3 other members. Would you like the detailed profile for any of them?


## ❓ FAQ

**Q: Can my agent list all connectors in a specific Fivetran group?**
Yes. Use the 'list_connectors' tool. Provide the Group ID, and the agent will return a list of all connectors configured within that destination group, including their unique IDs and statuses.

**Q: How do I check the details of a specific data destination via chat?**
Use the 'get_destination' tool. Provide the Group ID. Your agent will retrieve configuration details about the database or data warehouse connected to that group, providing clear boundary information natively.

**Q: Can I audit users and their roles in my Fivetran workspace through the agent?**
Absolutely. Use the 'list_users' tool. The agent retrieves all registered users in your workspace with their assigned roles and current statuses, allowing for organizational administrative auditing natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fivetran](https://vinkius.com/mcp/fivetran)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fivetran** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fivetran` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fivetran** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fivetran": {
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

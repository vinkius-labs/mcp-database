# Incident.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/incidentio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage incidents, roles, and on-call schedules via Incident.io API.

## Description
Empower your AI agents to manage your incident response lifecycle with Incident.io. This MCP server allows you to list and retrieve incidents, manage roles and types, track custom fields, and view on-call schedules directly through the Incident.io API. Ideal for automating SRE workflows and incident coordination.


## Available Tools
- **get_incident**: Retrieves details for a specific incident
- **list_catalog_types**: Lists all defined catalog types
- **list_custom_fields**: Lists all defined custom fields
- **list_incident_roles**: Lists all defined incident roles
- **list_incident_types**: Lists all defined incident types
- **list_incidents**: Lists all incidents
- **list_schedules**: Lists all on-call schedules
- **list_severities**: Lists all defined incident severities
- **list_teams**: Lists all teams
- **list_users**: Lists all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incident.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ongoing incidents in Incident.io."

**🤖 AI Agent:**
> I'll fetch the list of current incidents for you.

---

**👤 You:**
> "Show me the on-call schedules for this week."

**🤖 AI Agent:**
> I'll retrieve the active on-call schedules from Incident.io.

---

**👤 You:**
> "Check the details for incident ID 'abc-123'."

**🤖 AI Agent:**
> I'll look up the full details and history for that specific incident.


## ❓ FAQ

**Q: How do I get Incident.io API credentials?**
Log in to your Incident.io dashboard, navigate to Settings > API keys, and click 'Add new' to generate a Bearer Token.

**Q: Which version of the API is used?**
This MCP uses Incident.io API v2, the latest stable version for comprehensive incident management.

**Q: Can I see on-call schedules?**
Yes, the list_schedules tool provides access to on-call schedules and rotation information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incidentio](https://vinkius.com/mcp/incidentio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Incident.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `incidentio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Incident.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "incidentio": {
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

# Insightly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/insightly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage CRM contacts, opportunities, and projects via Insightly API.

## Description
Empower your AI agents to manage your customer relationships with Insightly. This MCP server allows you to list and retrieve contacts, organizations, opportunities, and projects directly through the Insightly API. Ideal for automating sales workflows and project tracking within your CRM.


## Available Tools
- **get_contact**: Retrieves details for a specific contact
- **list_contacts**: Lists all contacts in Insightly
- **list_events**: Lists all calendar events
- **list_leads**: Lists all marketing leads
- **list_opportunities**: Lists all sales opportunities
- **list_organisations**: Lists all registered organisations
- **list_projects**: Lists all active and past projects
- **list_tasks**: Lists all tasks across projects
- **list_teams**: Lists all defined teams
- **list_users**: Lists all users in the system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insightly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in Insightly."

**🤖 AI Agent:**
> I'll fetch your CRM contact directory for you.

---

**👤 You:**
> "Show me active projects in my Insightly account."

**🤖 AI Agent:**
> I'll retrieve the list of active and past projects from Insightly.

---

**👤 You:**
> "Check for any new sales opportunities."

**🤖 AI Agent:**
> I'll look up the current sales opportunities in your account.


## ❓ FAQ

**Q: How do I get Insightly API credentials?**
Log in to Insightly, click your profile icon, go to User Settings, and scroll down to the API Key section. You will also see your API URL which contains your pod (e.g., na1).

**Q: What is the 'pod'?**
The pod is the region identifier in your Insightly API URL, such as 'na1' for North America or 'eu1' for Europe.

**Q: Can I see sales opportunities?**
Yes, the list_opportunities tool provides access to all sales opportunities recorded in your Insightly account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/insightly](https://vinkius.com/mcp/insightly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insightly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `insightly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insightly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insightly": {
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

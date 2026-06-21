# Storylane MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/storylane)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Interactive, personalized product demos.

## Description
The Storylane MCP server connects your AI agent directly to your demo infrastructure. Query demo completion rates, create personalized demo links for prospects, and sync engagement data natively.


## Available Tools
- **create_demo_link**: Generate a new trackable demo link
- **get_demo_analytics**: Get engagement metrics for a specific demo
- **get_demo**: Get metadata and status for a specific demo
- **get_me**: Get information about the current authenticated user
- **get_session_details**: Get detailed information for a specific viewer session
- **get_workspace_info**: Retrieve metadata about the current Storylane workspace
- **list_demo_links**: Retrieve all active links associated with a specific demo
- **list_demos**: List all published demos in the workspace
- **list_sessions**: List granular session analytics for demo viewers
- **list_teams**: List teams within the workspace
- **list_users**: List all users and their roles in the workspace
- **update_demo_link**: Update settings for an existing demo link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storylane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active product demos."

**🤖 AI Agent:**
> You have 3 active demos: 'Platform Overview', 'Analytics Deep Dive', and 'Admin Panel'.

---

**👤 You:**
> "Create a personalized link for 'Analytics Deep Dive' for Acme Corp."

**🤖 AI Agent:**
> Personalized link generated: storylane.io/demo/acme-analytics-123

---

**👤 You:**
> "Show the completion rate for the 'Platform Overview' demo."

**🤖 AI Agent:**
> The 'Platform Overview' demo currently has a 68% completion rate with an average view time of 4m 12s.


## ❓ FAQ

**Q: Can I generate a personalized demo link?**
Yes! Provide the prospect's name and the base demo ID, and the agent will return a uniquely tracked URL.

**Q: How do I view the analytics for a specific demo?**
You can ask the AI to summarize views, completion rates, and the most clicked features of any published demo.

**Q: Is it possible to list all active demo flows?**
Yes, querying for active demos will return their titles, IDs, and current engagement scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storylane](https://vinkius.com/mcp/storylane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storylane** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `storylane` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storylane** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storylane": {
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

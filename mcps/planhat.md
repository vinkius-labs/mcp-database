# Planhat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planhat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer success via Planhat — list companies, track end users, and monitor tasks directly from any AI agent.

## Description
Connect your **Planhat** workspace to any AI agent and take full control of your customer success and growth workflows through natural conversation.

### What you can do

- **Company Oversight** — List all companies and retrieve detailed metadata to manage your customer relationships.
- **User & Contact Tracking** — List end users and associated metadata to understand your user base.
- **Task & Activity Management** — List pending tasks and monitor activities to ensure proactive customer management.
- **Conversation Discovery** — List all ongoing conversations to maintain a pulse on customer communication.
- **License & Asset Auditing** — List configured licenses and assets to verify customer entitlements.
- **Project Monitoring** — List active projects to track implementation and success plans.

### How it works

1. Subscribe to this server
2. Enter your Planhat API Token (from Settings > API)
3. Start managing your customers directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers (CSM)** — quickly check a company's health or verify pending tasks before a sync.
- **Account Executives** — lookup end user info and active licenses while preparing for renewals.
- **Operations Teams** — audit conversations and asset metadata directly from your chat interface.


## Available Tools
- **get_planhat_company**: Get details for a specific company
- **get_planhat_me**: Get current user info
- **list_planhat_assets**: List all assets
- **list_planhat_companies**: List all companies in Planhat
- **list_planhat_conversations**: List all conversations
- **list_planhat_end_users**: List all end users
- **list_planhat_licenses**: List all licenses
- **list_planhat_notes**: List all notes
- **list_planhat_projects**: List all projects
- **list_planhat_tasks**: List all tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planhat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active companies in my Planhat account."

**🤖 AI Agent:**
> I've retrieved 15 active companies, including 'Acme Corp', 'Global Tech', and 'Startup Inc'. Would you like details for any specific company?

---

**👤 You:**
> "Show me the last 5 tasks assigned to me in Planhat."

**🤖 AI Agent:**
> I've fetched your latest tasks. They include 'Review renewal for Acme', 'Setup sync with Global Tech', and 3 other items. Would you like to see the due dates?

---

**👤 You:**
> "What are the active licenses for company 'Acme Corp'?"

**🤖 AI Agent:**
> Acme Corp currently has 3 active licenses: 'Enterprise Platform', 'Advanced Analytics Add-on', and 'Premium Support'. All are valid until Dec 2026.


## ❓ FAQ

**Q: How do I find my Planhat API Token?**
In your Planhat account, go to **Settings** > **API**. There you can generate and copy your security token.

**Q: Can I see all end users for a specific company?**
Yes! Use the `list_planhat_end_users` tool. You can then ask the AI agent to filter the results for a particular company name or ID from the retrieved list.

**Q: Does this support checking active licenses?**
Absolutely. Use the `list_planhat_licenses` tool to retrieve a comprehensive list of all customer licenses and their associated data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planhat](https://vinkius.com/mcp/planhat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Planhat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `planhat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Planhat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planhat": {
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

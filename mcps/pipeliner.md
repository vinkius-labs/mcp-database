# Pipeliner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipeliner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage sales pipelines and opportunities via Pipeliner CRM — list leads, track deals, and monitor activities directly from any AI agent.

## Description
Connect your **Pipeliner CRM** space to any AI agent and take full control of your sales ecosystem through natural conversation.

### What you can do

- **Lead & Opportunity Oversight** — List and retrieve detailed metadata for leads and sales opportunities across your workspace.
- **Sales Pipeline Management** — List available pipelines and track the progress of deals through different stages.
- **Workforce Visibility** — List company accounts, business contacts, and team members to maintain a clear view of your stakeholders.
- **Activity & Task Tracking** — Monitor sales activities and assigned tasks to ensure your team stays productive.
- **Detailed Entity Inspections** — Get deep-dive details for any specific lead or opportunity to understand its full history.

### How it works

1. Subscribe to this server
2. Enter your Pipeliner API Token, Space ID, and Service URL
3. Start managing your sales directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Managers** — quickly check the status of a specific opportunity or audit team activities without opening the CRM.
- **Account Executives** — lookup contact details and recent leads while preparing for client meetings.
- **Sales Ops** — monitor pipeline structures and task assignments directly from your chat interface.


## Available Tools (10)
- **get_pipeliner_lead**: Get details for a specific lead
- **get_pipeliner_opportunity**: Get details for a specific opportunity
- **list_pipeliner_accounts**: List all company accounts
- **list_pipeliner_activities**: List sales activities and tasks
- **list_pipeliner_contacts**: List all business contacts
- **list_pipeliner_leads**: List all sales leads
- **list_pipeliner_opportunities**: List all sales opportunities
- **list_pipeliner_pipelines**: List available sales pipelines
- **list_pipeliner_tasks**: List all assigned tasks
- **list_pipeliner_users**: List users in the Pipeliner space


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeliner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sales opportunities in the 'Enterprise' pipeline."

**🤖 AI Agent:**
> I've retrieved 6 opportunities from the 'Enterprise' pipeline. Total value is $245,000. Key deals include 'Global Bank Cloud Migration' and 'City Gov ERP Phase 2'.

---

**👤 You:**
> "Show me the last 5 leads added to Pipeliner."

**🤖 AI Agent:**
> I've fetched the latest leads. Recent additions include 'Tech Solutions Inc', 'Retail Group Asia', and 3 others. Would you like their contact info or lead status?

---

**👤 You:**
> "What are my sales activities for this week?"

**🤖 AI Agent:**
> You have 12 activities scheduled this week: 5 follow-up calls, 3 discovery meetings, and 4 internal tasks. Would you like a daily breakdown?


## ❓ FAQ

**Q: How do I find my Pipeliner Space ID and Service URL?**
Log in to Pipeliner, go to **Admin Space** > **API**. There you can find your unique Space ID and the specific API Service URL for your instance.

**Q: Can I see opportunities across multiple pipelines?**
Yes! Use the `list_pipeliner_opportunities` tool to retrieve a full list of deals. You can then ask the AI agent to filter or group them by pipeline name.

**Q: Does this support looking up individual user activities?**
Absolutely. Use the `list_pipeliner_activities` tool to retrieve a log of all sales tasks, calls, and meetings recorded in your CRM space.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipeliner](https://vinkius.com/mcp/pipeliner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeliner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeliner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeliner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeliner": {
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

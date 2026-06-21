# Pipeline CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipeline-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage sales and contacts via Pipeline CRM — list deals, track people, and monitor tasks directly from any AI agent.

## Description
Connect your **Pipeline CRM** account to any AI agent and take full control of your sales pipeline and contact management through natural conversation.

### What you can do

- **Contact Oversight** — List all people and companies in your CRM and retrieve detailed profile metadata.
- **Sales Pipeline Tracking** — List and retrieve details for all active deals to stay on top of your revenue goals.
- **Task & Event Management** — List pending tasks and calendar events to organize your daily sales activities.
- **Note & Comment Auditing** — Retrieve recent notes and comments to understand the history of any lead or deal.
- **User & Account Visibility** — List account users and retrieve global settings to maintain visibility over your team's access.

### How it works

1. Subscribe to this server
2. Enter your Pipeline CRM API Key (from account settings)
3. Start managing your sales directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Representatives** — quickly lookup contact info or check the status of a deal while preparing for a call.
- **Sales Managers** — monitor team tasks and recent notes to audit pipeline progress.
- **Account Executives** — verify company details and upcoming calendar events directly from your chat interface.


## Available Tools
- **get_pipeline_account**: Get account settings and info
- **get_pipeline_deal**: Get details for a specific deal
- **get_pipeline_person**: Get details for a specific person
- **list_pipeline_companies**: List companies in the CRM
- **list_pipeline_deals**: List sales deals
- **list_pipeline_events**: List calendar events
- **list_pipeline_notes**: List recent notes/comments
- **list_pipeline_people**: List people in Pipeline CRM
- **list_pipeline_tasks**: List pending tasks
- **list_pipeline_users**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active deals in my sales pipeline."

**🤖 AI Agent:**
> I've retrieved your deals. You have 5 active ones, including 'Enterprise Upgrade' ($50,000) and 'Startup Onboarding' ($12,000). Would you like more details on any of these?

---

**👤 You:**
> "Show me the last 5 people added to my contacts."

**🤖 AI Agent:**
> I've fetched the latest contacts. The most recent additions are 'Alice Johnson', 'Bob Smith', and 3 others. Would you like their email addresses or company info?

---

**👤 You:**
> "What tasks are assigned to me for today?"

**🤖 AI Agent:**
> You have 3 tasks for today: 'Follow up with Acme Corp', 'Send proposal to GlobalTech', and 'Review Q4 goals'.


## ❓ FAQ

**Q: How do I find my Pipeline CRM API Key?**
Log in to Pipeline CRM, go to **Account Settings** > **Integrations** > **API**. There you can find and copy your API Key.

**Q: Can I see all my deals across different stages?**
Yes! Use the `list_pipeline_deals` tool to retrieve a comprehensive list of all active deals and their current pipeline stage.

**Q: Does this support looking up company information?**
Absolutely. Use the `list_pipeline_companies` tool to retrieve a list of all organizations stored in your CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipeline-crm](https://vinkius.com/mcp/pipeline-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pipeline-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-crm": {
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

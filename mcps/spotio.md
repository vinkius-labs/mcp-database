# Spotio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spotio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage leads, pipelines, and field sales activities on Spotio with AI agents.

## Description
Connect your **Spotio** account to any AI agent to automate your field sales and outside sales management. Spotio provides a premier platform for territory management and lead tracking, and this integration allows you to retrieve lead metadata, monitor pipelines, and track field visits through natural conversation.

### What you can do

- **Lead & Prospect Orchestration** — List all managed leads and retrieve detailed profile metadata, including status and contact info programmatically.
- **Pipeline Lifecycle Management** — Access and monitor your sales pipelines and stages to ensure your sales funnel is always synchronized directly from the AI interface.
- **Activity & Visit Tracking** — Retrieve real-time field visit data and monitor sales activities to track team performance via natural language.
- **User & Team Oversight** — Access and monitor team members and their activity logs to maintain a clear overview of your field operations.
- **Webhook & Automation Intelligence** — List and manage webhooks to ensure your sales data is instantly notified across your business stack.

### How it works

1. Subscribe to this server
2. Enter your Spotio Client ID and Secret from your account settings
3. Start managing your field sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Field Sales Managers** — quickly retrieve lead details and monitor team visit logs without switching apps.
- **Operations Leads** — automate the management of pipelines and track field activities via natural conversation.
- **Sales Development Teams** — streamline the retrieval of lead metadata and coordinate pipeline stages directly within the chat.


## Available Tools (12)
- **create_lead**: Create a new lead
- **create_webhook**: status.changed.

Create a new webhook
- **get_account_info**: Get current user profile
- **get_lead**: Get lead details
- **list_lead_activities**: List lead activities
- **list_leads**: List all sales leads
- **list_pipelines**: List sales pipelines
- **list_pipeline_stages**: List pipeline stages
- **list_team_users**: List team users
- **list_field_visits**: List field visits
- **list_webhooks**: List configured webhooks
- **update_lead**: Update lead info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spotio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads in Spotio."

**🤖 AI Agent:**
> I've retrieved your lead list. You have 45 active prospects in your current territory, including 'John Smith' (High Priority) and 'Acme Supplies'. Would you like to check the pipeline status for any of them?

---

**👤 You:**
> "Show me the field sales team activity with visits logged, deals closed, and territory coverage this week."

**🤖 AI Agent:**
> Field sales activity this week. 12 reps active. Total visits: 345 (avg 28.8/rep). Doors knocked: 890. Meetings held: 123. Deals closed: 34 ($234,000 total). Top rep: Sarah Chen (45 visits, 8 deals, $67,000). Territory coverage: North (89% mapped), South (76%), East (82%), West (71%). GPS tracks logged: 2,340 miles driven. Average time per visit: 18 minutes. Pipeline generated: $890K from new leads. Follow-ups scheduled: 89. No-answers: 234 (26.3% of doors knocked).

---

**👤 You:**
> "Create a new sales territory assignment for the downtown business district with lead pins."

**🤖 AI Agent:**
> Territory created: "Downtown Business District". Boundaries: defined by 4 GPS coordinates (polygon). Assigned to: James Park (senior rep). Existing leads imported: 234 pins (from CRM). Lead categories: Hot (23, red pins), Warm (67, yellow), Cold (144, blue). Businesses mapped: 456 (from Google Places). Not yet contacted: 222 (48.7%). Last visit data: 89 businesses visited in past 90 days. Route optimization: 3 suggested daily routes (8-12 stops each). Estimated coverage time: 2 weeks for full territory.


## ❓ FAQ

**Q: How do I find my Spotio API credentials?**
Log in to your Spotio account and navigate to the developer or API settings section to generate your unique Client ID and Secret.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spotio](https://vinkius.com/mcp/spotio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spotio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spotio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spotio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spotio": {
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

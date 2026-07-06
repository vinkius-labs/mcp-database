# Reportei MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reportei)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate marketing performance reports from Google, Facebook, and Instagram data in minutes for client presentations.

## Description
Connect your **Reportei** account to any AI agent and take full control of your digital marketing orchestration and reporting workflows through natural conversation. Reportei provides a premier platform for consolidating metrics from social networks and ad platforms, and this integration allows you to retrieve project metadata, monitor report generation, and log important timeline events directly from your chat interface.

### What you can do

- **Project & Client Orchestration** — List all managed marketing projects and retrieve detailed client metadata programmatically.
- **Report & Analysis Intelligence** — Access and monitor generated reports and retrieve detailed performance metadata directly from the AI interface.
- **Metric & Performance Tracking** — Retrieve real-time data from connected channels like Instagram, Facebook, and Google Ads via natural language.
- **Timeline & Event Control** — Create and list project timeline events to maintain a comprehensive history of marketing actions and results.
- **Operational Monitoring** — Track system activity and manage project settings using simple AI commands to ensure your reporting is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Reportei API Token from your account settings
3. Start managing your marketing reports from Claude, Cursor, or any MCP-compatible client

No more manual data collection or complex spreadsheet reporting. Your AI acts as a dedicated marketing analyst or account coordinator.

### Who is this for?

- **Marketing Agencies** — quickly retrieve client results and monitor project timelines without switching apps.
- **Social Media Managers** — automate the extraction of performance metrics and track campaign milestones via natural conversation.
- **Data Analysts** — streamline the retrieval of consolidated marketing data directly within the chat.


## Available Tools (10)
- **get_reportei_metrics**: Get raw metrics data
- **get_report_details**: Get details for a specific report
- **list_clients**: List all clients
- **list_integrations**: List all connected integrations
- **list_reportei_projects**: List all marketing projects
- **list_reportei_reports**: You can filter by project ID.

List generated reports
- **list_reportei_timeline**: List timeline events
- **create_report**: Generate a new analytics report
- **add_reportei_event**: Add a timeline event
- **get_client**: Get details for a specific client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reportei** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing projects in my Reportei account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active environments including 'Vinkius Growth' and 'Social Media Client A'. Which one would you like to see metrics for?

---

**👤 You:**
> "Generate a comprehensive marketing report for all social media channels from last month."

**🤖 AI Agent:**
> Marketing report generated for April 2025. Instagram: 12,400 followers (+3.2%), 234K reach, 8,900 engagements (4.1% rate). Facebook: 8,900 page likes, 156K reach, 3,400 engagements. LinkedIn: 5,600 followers (+5.8%), 89K impressions, 1,200 engagements. Twitter/X: 4,200 followers, 67K impressions. TikTok: 2,800 followers (+12%), 445K views. Cross-channel totals: 997K total reach, 14,700 engagements. Top performing post: Instagram Reel with 45K views. Report exported as PDF with charts.

---

**👤 You:**
> "Show me all projects and their connected integrations with data freshness status."

**🤖 AI Agent:**
> 8 active projects. "Main Brand" has 6 integrations: Google Analytics (synced 2h ago), Instagram (synced 1h ago), Facebook (synced 1h ago), LinkedIn (synced 3h ago), Google Ads (synced 2h ago), YouTube (synced 4h ago). "Client: Meridian" has 4 integrations: Google Analytics, Instagram, Facebook, Google Ads (all synced within 2h). "Client: TechFlow" has 3 integrations. 5 additional client projects with combined 18 integrations. All connections healthy. 1 integration warning: LinkedIn token expires in 5 days.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific project just by providing its ID?**
Yes! Use the `list_reportei_projects` tool. Your agent will respond with complete metadata for all your projects, allowing you to identify and inspect individual client accounts in seconds.

**Q: How do I find my Reportei API Token?**
Log in to your Reportei account, navigate to **Settings** > **Company** > **Reportei API**, and you will find your unique secret token there.

**Q: Can I retrieve metrics for a specific date range?**
Yes, using the `get_reportei_metrics` tool, you can provide `start_date` and `end_line` parameters to fetch consolidated marketing data for any specific period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reportei](https://vinkius.com/mcp/reportei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reportei** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reportei` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reportei** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reportei": {
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

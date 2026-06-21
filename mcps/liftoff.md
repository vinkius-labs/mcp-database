# Liftoff MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liftoff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access mobile advertising performance reports and metadata via the Liftoff REST API.

## Description
Connect your **Liftoff** (formerly Vungle) advertising account to any AI agent to automate your mobile marketing analytics and reporting. This MCP server enables your agent to list campaigns, request detailed performance reports, and monitor spend in real-time directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all apps, campaigns, and creative assets to map performance IDs to readable names
- **Automated Reporting** — Request asynchronous performance reports (v1) for deep dives into historical data
- **Real-time Spend** — Query synchronous spend and install metrics (v2) for immediate operational awareness
- **Lifecycle Tracking** — Monitor the status of report generation and download completed results effortlessly
- **Dimension Filtering** — Filter your data by app, campaign, country, and platform to identify growth opportunities

### How it works

1. Subscribe to this server
2. Enter your Liftoff API Key and API Secret
3. Start managing your advertising data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UA Managers** — Monitor campaign performance and spend totals via simple natural language commands
- **Data Analysts** — Automate the extraction of advertising metadata and performance logs into your workflow
- **Growth Marketers** — Quickly check recent install trends and click-through rates across different countries


## Available Tools
- **list_liftoff_apps**: List all applications in your Liftoff account
- **list_liftoff_campaigns**: List all advertising campaigns
- **request_performance_report**: Requires start and end dates.

Initialize a performance report request (v1)
- **list_liftoff_creatives**: List all creative assets
- **download_report_results**: Retrieve the data for a completed report
- **get_report_status**: Check the status of a requested report
- **get_spend_metrics**: Get a synchronous spend and performance report (v2)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liftoff** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active advertising campaigns in Liftoff."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 12 active campaigns, including 'Spring Sale 2024', 'iOS Retargeting', and 'Android Global Launch'. Which one would you like to see metrics for?

---

**👤 You:**
> "Show recent spend and installs for campaign ID 'camp-123'."

**🤖 AI Agent:**
> I've queried the spend report. For campaign 'camp-123' today, you've spent $1,250.00 and generated 450 installs with a conversion rate of 3.2%.

---

**👤 You:**
> "Request a performance report for the month of July in JSON format."

**🤖 AI Agent:**
> I've submitted the report request for July (Start: 2024-07-01, End: 2024-07-31). The report ID is 'rep-98765'. I will monitor its status for you.


## ❓ FAQ

**Q: How do I get my API Key and Secret?**
You must contact your Liftoff (Vungle) Account Manager to receive your specialized Reporting API credentials.

**Q: What is the difference between Reporting v1 and v2?**
Reporting v1 is asynchronous and used for large, detailed historical datasets. Reporting v2 is synchronous and provides quick access to spend and install metrics.

**Q: Can I filter data by country?**
Yes, by including 'country' in the `dimensions` parameter of the spend report, or by configuring the group_by settings in a v1 report request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liftoff](https://vinkius.com/mcp/liftoff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liftoff** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `liftoff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liftoff** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liftoff": {
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

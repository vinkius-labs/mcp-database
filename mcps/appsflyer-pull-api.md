# AppsFlyer (Pull API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appsflyer-pull-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Retrieve raw and aggregate attribution data from AppsFlyer — track installs, events, and performance via AI.

## Description
The **AppsFlyer Pull API MCP Server** provides your AI agent with direct access to your mobile attribution and marketing analytics data. Effortlessly retrieve raw reports for installs and in-app events, or get aggregate performance metrics by day, geography, or media source using natural language.

### Key Features

- **Raw Data Retrieval** — Download non-organic installs, in-app events, and uninstalls reports for granular analysis.
- **Aggregate Reporting** — Access high-level performance summaries by partner (media source), geography, or day.
- **Customizable Timeframes** — Specify exact start and end dates for any report to focus on specific campaigns or periods.
- **CSV Output Support** — Reports are delivered in structured CSV format, allowing for further data processing or direct review.
- **Security & Privacy** — Uses AppsFlyer API Token V2 (JWT) for secure, authenticated access to your data.

### Who is this for?

- **UA Managers** — Quickly audit campaign performance and install trends across different partners.
- **Data Analysts** — Retrieve raw event data for deeper investigation into user behavior and LTV.
- **Growth Marketers** — Monitor daily performance and geographic trends to optimize spend and targeting.


## Available Tools (7)
- **get_account_check**: Verify AppsFlyer account connection
- **get_daily_report**: Get aggregate daily performance report
- **get_geo_report**: Get aggregate performance report by geography
- **get_in_app_events_report**: Get in-app events raw data report
- **get_installs_report**: Get non-organic installs raw data report
- **get_partners_report**: Get aggregate performance report by media source
- **get_uninstalls_report**: Get uninstalls raw data report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppsFlyer (Pull API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the installs report for last week."

**🤖 AI Agent:**
> I've retrieved your installs report for the last 7 days. It includes details for 1,250 non-organic installs from various media sources.

---

**👤 You:**
> "Show me the aggregate daily performance for February 2024."

**🤖 AI Agent:**
> I've pulled the daily performance report for February. You had a total of 15,400 installs and 45,000 sessions during this period.

---

**👤 You:**
> "Retrieve in-app events data for today."

**🤖 AI Agent:**
> The in-app events report for today has been retrieved. There are 250 records so far, including 'purchase' and 'level_complete' events.


## ❓ FAQ

**Q: How do I find my AppsFlyer API Token V2?**
Log in to AppsFlyer as an Admin, go to **Security Center** from the account menu, and navigate to **AppsFlyer API tokens**. There you can manage and copy your V2 token (JWT).

**Q: What is the 'appId'?**
The `appId` is the unique identifier for your app in the store. For iOS, it's usually `id` followed by numbers (e.g., `id123456789`). For Android, it's the package name (e.g., `com.example.app`).

**Q: Is there a limit on the number of rows returned?**
Yes, AppsFlyer Pull API limits raw data reports to 200,000 rows. If your data exceeds this, try narrowing the date range of your request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appsflyer-pull-api](https://vinkius.com/mcp/appsflyer-pull-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppsFlyer (Pull API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appsflyer-pull-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppsFlyer (Pull API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appsflyer-pull-api": {
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

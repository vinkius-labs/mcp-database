# AppLovin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/applovin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your AppLovin and MAX advertising performance — track revenue, impressions, and campaigns via AI.

## Description
The **AppLovin MCP Server** provides your AI agent with a powerful interface to your AppLovin and MAX mediation platforms. Gain instant insights into your monetization and user acquisition performance using simple natural language.

### Key Features

- **MAX Reporting** — Access aggregated performance data for your MAX mediation, including revenue, impressions, and eCPM.
- **User-Level Insights** — Retrieve detailed revenue reports aggregated per user or per impression for granular analysis.
- **Cohort Analytics** — Monitor user retention and long-term value using MAX cohort reports.
- **AppDiscovery Management** — Track the performance of your UA campaigns and monitor growth trends.
- **Campaign & App Inventory** — List all active campaigns and tracked apps in your AppLovin account.
- **Multi-Key Authentication** — Securely uses both Report and Management keys to provide a comprehensive set of tools.

### Benefits for Teams

- **Ad Ops Managers** — Quickly audit monetization performance and eCPM trends without manual dashboard exports.
- **UA Specialists** — Monitor campaign spend and performance across AppDiscovery using natural language.
- **Growth Engineers** — Analyze user-level revenue and cohort data to optimize long-term retention and ROI.


## Available Tools (7)
- **get_account_check**: Verify AppLovin account connection
- **get_user_ad_revenue_report**: Get revenue data aggregated per user or per impression
- **get_app_discovery_report**: Get performance data for UA campaigns (AppDiscovery)
- **get_max_cohort_report**: Get cohort analysis reports for MAX
- **get_max_report**: Use columns, start, and end parameters.

Get aggregated performance data for MAX mediation
- **list_apps**: List apps tracked in your AppLovin account
- **list_campaigns**: List UA campaigns from the management API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppLovin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the MAX revenue report for yesterday."

**🤖 AI Agent:**
> Your MAX revenue yesterday was $1,250.40 with 450,000 impressions and an eCPM of $2.78.

---

**👤 You:**
> "List all active UA campaigns in AppLovin."

**🤖 AI Agent:**
> I've retrieved your active campaigns. You have 8 campaigns running, including 'WordPuzzle_iOS_US' and 'WordPuzzle_Android_Global'.

---

**👤 You:**
> "Give me a cohort report for user retention from last month."

**🤖 AI Agent:**
> The cohort report for last month shows a Day 1 retention of 42% and a Day 7 retention of 18% for your main app.


## ❓ FAQ

**Q: Where do I find my AppLovin API keys?**
You can find your Report Key and Management Key in the AppLovin dashboard under **Account > Keys**.

**Q: What is the difference between the Report Key and Management Key?**
The Report Key is used for read-only access to performance data, while the Management Key is required for making changes to campaigns and ad units.

**Q: How often is user-level data updated?**
User-level ad revenue data is typically available approximately 8 hours after the end of the UTC day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/applovin](https://vinkius.com/mcp/applovin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppLovin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `applovin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppLovin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "applovin": {
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

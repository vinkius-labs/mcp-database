# CallGear MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callgear)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze communication performance via CallGear — track calls, monitor advertising campaigns, and retrieve real-time stats directly from any AI agent.

## Description
Connect your **CallGear** account to any AI agent and orchestrate your communication analytics, marketing attribution, and call tracking through natural conversation.

### What you can do

- **Call Performance Oversight** — Retrieve detailed reports of all incoming and outgoing calls, including sources, durations, and statuses.
- **Marketing Attribution** — Monitor advertising campaign performance and identify which sources are driving the most communications.
- **Communication Analysis** — Get broader reports covering calls, chats, and other interactions to ensure service quality.
- **Infrastructure Coordination** — Access and monitor your traffic sources, call scenarios, and tags directly from your workspace.
- **User & Team Oversight** — List all users in your CallGear account to maintain visibility across your team.
- **Real-time Statistics** — Retrieve daily site and campaign stats straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your CallGear Data API Access Token
3. Start analyzing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Analysts** — quickly check campaign performance or traffic sources without manual report exporting.
- **Sales Managers** — monitor call durations and team activity straight from their workflow tools.
- **Business Admins** — retrieve daily communication summaries and account info using natural language.


## Available Tools
- **get_account_info**: Retrieve core account information
- **get_ad_campaigns_report**: Retrieve daily aggregated statistics for advertising campaigns
- **get_calls_report**: Retrieve a detailed report of calls for a specific period
- **get_communications_report**: Retrieve a report covering various communication types (calls, chats, etc.)
- **get_site_daily_stats**: Retrieve daily statistics for sites
- **list_ad_campaigns**: List all advertising campaigns
- **list_call_scenarios**: List all configured call scenarios
- **list_traffic_sources**: List all traffic sources configured in CallGear
- **list_tags**: List all call and communication tags
- **list_users**: List all users in the CallGear account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallGear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the calls report from March 1st to March 7th."

**🤖 AI Agent:**
> I've retrieved the calls report. You had 150 incoming calls in that period, with an average duration of 2m 30s. The most common source was 'Google Ads'.

---

**👤 You:**
> "Which advertising campaigns are active right now?"

**🤖 AI Agent:**
> Retrieving active campaigns... You have 3 campaigns running: 'Spring Sale 2026', 'Search Network - Leads', and 'Retargeting Display'.

---

**👤 You:**
> "Show daily stats for my website for the last 3 days."

**🤖 AI Agent:**
> Retrieving site stats... In the last 3 days, you averaged 50 unique communications per day, with 85% being voice calls and 15% chats.


## ❓ FAQ

**Q: Can I check the calls report for a specific week using the agent?**
Yes! Use the `get_calls_report` tool and provide the `date_from` and `date_to` parameters. Your agent will fetch the detailed breakdown of all communications for that period.

**Q: How do I see which marketing source is generating the most calls?**
Simply ask the agent to `get_ad_campaigns_report` or `get_calls_report`. It will retrieve the statistics grouped by source or campaign, allowing you to analyze attribution instantly.

**Q: Does the integration allow listening to call recordings?**
The current toolset focuses on data analytics and metadata retrieval. To listen to recordings, you should use the links provided in the CallGear dashboard or check the `link_to_record` field if available in the report results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callgear](https://vinkius.com/mcp/callgear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CallGear** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `callgear` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CallGear** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "callgear": {
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

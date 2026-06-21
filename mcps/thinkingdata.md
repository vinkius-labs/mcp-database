# ThinkingData / 数数科技 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkingdata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Dominant games and app analytics platform — query events, audit users, and track data via AI.

## Description
Empower your AI agent to orchestrate your data analytics and player insights with **ThinkingData** (数数科技), the premier analytics platform for the global gaming industry. By connecting ThinkingData to your agent, you transform complex event querying, user profile auditing, and cohort management into a natural conversation. Your agent can instantly retrieve project metadata, list defined events and their schemas, execute complex behavioral queries, and even ingest custom events without you ever needing to navigate the comprehensive TA Dashboard. Whether you are conducting a player retention audit or coordinating a live-ops event refresh, your agent acts as a real-time data coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Project Orchestration** — Retrieve project summaries, list defined events, and discover property schemas.
- **Behavioral Auditing** — Execute complex queries on event data to understand player behavior and conversion funnels.
- **User Management** — Query user profile data and update properties for specific distinct IDs.
- **Data Ingestion** — Track custom events and set user properties directly through the agent for rapid testing.
- **Operational Insights** — List defined user cohorts, saved reports, and monitor API connectivity status.

### How it works

1. Subscribe to this server
2. Enter your TA Project APPID, Data Token, Query Secret, and API URL
3. Start managing your data analytics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Data Analysts** — automate routine event queries and report generation through natural language.
- **Live-Ops Managers** — monitor real-time player behavior and verify event tracking directly from your workspace.
- **Developers** — integrate professional-grade gaming analytics into your AI-driven daily routines.
- **ThinkingAnalytics Power Users** — integrate your existing analytics workflows into your AI-driven daily routines.


## Available Tools
- **get_event_properties**: Get properties for event
- **get_project_summary**: Get project overview
- **list_defined_events**: List project events
- **list_project_cohorts**: List user cohorts
- **query_events**: Execute event query
- **query_users**: Execute user query
- **set_user_properties**: Update user profile
- **track_custom_event**: Track a single event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThinkingData / 数数科技** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a summary of our ThinkingData project configuration."

**🤖 AI Agent:**
> I've retrieved the project summary. Your project 'Global_Quest_01' is currently active on the China-East data center. There are 45 unique events defined and 12 active cohorts. Would you like me to list the most frequent events?

---

**👤 You:**
> "List all defined events in ThinkingData."

**🤖 AI Agent:**
> I've retrieved the event metadata. You have events like 'UserLogin', 'LevelUp', 'PurchaseStart', and 'TutorialComplete'. Should I show you the properties associated with the 'PurchaseStart' event?

---

**👤 You:**
> "Check the profile for user 'USER_88210934'."

**🤖 AI Agent:**
> I've queried the user profile. USER_88210934 has a total level of 42, last logged in 2 hours ago, and belongs to the 'VIP_Gold' cohort. Would you like me to update any of their properties?


## ❓ FAQ

**Q: How do I find my TA Project APPID and Tokens?**
Log in to your [ThinkingAnalytics Console](https://www.thinkingdata.cn/), go to [Project Management] -> [Project Info] to find your APPID and Data Token. The Query Secret is usually found in the [Account Management] or [API Management] section.

**Q: What is the 'distinctId'?**
The `distinctId` is the unique identifier for a user in your system (e.g., a device ID or an account ID). It is used to tie events and properties to a specific individual profile in ThinkingAnalytics.

**Q: Can I perform complex data analysis through the agent?**
Yes! Use the `query_events` tool with a JSON query definition. Your agent will fetch the raw or aggregated results from TA, allowing you to audit behavioral patterns using natural language reasoning over the returned data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkingdata](https://vinkius.com/mcp/thinkingdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThinkingData / 数数科技** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `thinkingdata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThinkingData / 数数科技** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thinkingdata": {
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

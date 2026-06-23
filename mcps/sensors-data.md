# Sensors Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sensors-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate Sensors Data analytics — manage events, query user profiles, and monitor data ingestion directly from any AI agent.

## Description
Connect your AI agents to **Sensors Data** (神策数据), the leading professional big data analytics platform. This MCP provides 10 tools to manage event tracking, retrieve user behavioral profiles, and monitor the health of your data pipeline directly through natural conversation.

### What you can do

- **Event Orchestration** — Query and analyze event metadata and properties to understand user interactions in real-time
- **User Profiling** — Retrieve detailed behavioral profiles and attributes for specific user IDs to power personalized experiences
- **Data Health** — Monitor ingestion rates and check for data quality issues across your analytics streams
- **Project Management** — List and inspect project configurations, including project names and token settings
- **Export Intelligence** — Trigger and monitor data export tasks for further downstream processing or reporting

### How it works

1. Subscribe to this server
2. Log in to your [**Sensors Data Dashboard**](https://www.sensorsdata.cn/)
3. Navigate to **Project Settings > API Access** to obtain your **Project Name** and **API Key** (Token)
4. Identify your **Base URL** (e.g., `https://api.sensorsdata.cn` or your private cloud endpoint)
5. Insert your credentials into the fields below to start managing your big data workflows.

### Who is this for?

- **Data Analysts** — automate the retrieval of user behavior metrics and event summaries via natural language
- **Product Managers** — monitor real-time feature adoption and user retention data without complex SQL
- **Growth Engineers** — integrate deep behavioral insights into automated marketing and personalization flows


## Available Tools (10)
- **analyze_events**: Perform complex event analysis
- **analyze_funnel**: Calculate conversion funnel metrics
- **analyze_retention**: Calculate user retention rates
- **get_event_schema**: Retrieve the property schema for a specific event
- **get_project_info**: Retrieve Sensors Data project metadata
- **get_user_behavior_sequence**: Get the chronological sequence of events for a user
- **list_events**: List all defined event names in the schema
- **list_user_properties**: List all defined user profile properties
- **lookup_user**: Get profile information for a specific user
- **query_behavior_list**: Retrieve a list of user behaviors/events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sensors Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 events by volume in project 'MainApp' for today."

**🤖 AI Agent:**
> Retrieving event statistics for 'MainApp'... The top 5 events today are: 1. page_view (1.2M), 2. item_click (450K), 3. user_login (120K), 4. add_to_cart (85K), 5. purchase_complete (12K). Would you like to see the conversion rate between these?

---

**👤 You:**
> "Get the behavioral attributes for user ID 'user_sensors_777'."

**🤖 AI Agent:**
> Querying user profile... User 'user_sensors_777' is categorized as a 'High-Value Customer' with 15 purchases in the last 30 days. Preferred category: 'Electronics'. Last active: 10 minutes ago.

---

**👤 You:**
> "Is the data ingestion pipeline healthy for project 'AnalyticsBeta'?"

**🤖 AI Agent:**
> Checking pipeline health for 'AnalyticsBeta'... Current status: Healthy. Ingestion rate is 15K events/sec with zero reported errors in the last hour. Connectivity to the Sensors Data cluster is stable.


## ❓ FAQ

**Q: Can I automatically retrieve the behavioral profile for a specific user ID?**
Yes! Use the `get_user_profile` tool with the specific User ID. Your agent will return all recorded attributes and recent behavioral events associated with that user.

**Q: How do I monitor the data ingestion status via the AI agent?**
Use the `get_ingestion_health` tool. The agent will retrieve real-time statistics on data volume, successful ingestions, and any flagged errors in your pipeline.

**Q: Can I list all events tracked in a specific project?**
Yes! Use the `list_events` tool. Your agent will return a list of all event names and their associated metadata currently configured in your Sensors Data project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sensors-data](https://vinkius.com/mcp/sensors-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sensors Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sensors-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sensors Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sensors-data": {
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

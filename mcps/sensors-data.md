# Sensors Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sensors-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sensors-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sensors-data-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Sensors Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sensors-data](https://vinkius.com/mcp/sensors-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# ThinkingData / 数数科技 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkingdata)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thinkingdata-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thinkingdata-mcp)
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


## Installation & Usage

To install and use the **ThinkingData / 数数科技** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkingdata](https://vinkius.com/mcp/thinkingdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

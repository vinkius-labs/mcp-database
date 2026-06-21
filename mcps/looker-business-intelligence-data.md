# Looker (Business Intelligence & Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/looker-business-intelligence-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/looker-business-intelligence-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/looker-business-intelligence-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your BI environment via Looker — list dashboards, execute inline queries, and audit saved Looks.

## Description
Connect your **Looker** instance to any AI agent and take full control of your enterprise business intelligence and data analytics through natural conversation.

### What you can do

- **Dashboard Orchestration** — List all managed dashboards and retrieve detailed configuration metrics and query structures directly from your agent
- **Dynamic Data Queries** — Execute inline queries against specific models and views to fetch literal dimensions and measures in real-time
- **Look & Report Audit** — Access saved 'Looks' to retrieve model mappings and applied filters for consistent data reporting across your organization
- **Content & Folder Search** — Search through content metadata and navigate folder hierarchies to identify key datasets and analytical assets securely
- **Metadata Inspection** — Extract precise UUIDs and configuration trees for dashboards and looks to understand the underlying data logic
- **Resource Inventory** — Enumerate root folders and top-level models to audit permissions and organizational structure across your Looker tenant

### How it works

1. Subscribe to this server
2. Enter your Looker Base URL, Client ID, and Client Secret
3. Start exploring your data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — verify dashboard configurations and run rapid inline queries through natural conversation without manual SQL exports
- **Business Users** — search for specific reports and retrieve rapid data summaries directly from your workspace
- **Platform Engineers** — audit content metadata access and manage folder hierarchies across multiple Looker environments efficiently


## Available Tools
- **list_dashboards**: List Looker dashboards
- **get_dashboard**: Get complete details and queries mapping a Looker Dashboard ID
- **list_looks**: List saved specific dataset mappings tracked as Looks
- **get_look**: Get full mapped details tracing a strict Looker target Look object
- **list_folders**: List root Folders analyzing explicit environment structures
- **search_content**: Search content metadata explicit mapping targets natively across instance
- **run_inline_query**: Execute queries building models specifically fetching literal dimensions dynamically natively


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Looker (Business Intelligence & Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 dashboards created in my Looker instance"

**🤖 AI Agent:**
> I've retrieved the 5 most recent dashboards. Highlights include 'Q1 Sales Overview' (ID: 123), 'User Engagement Deep-Dive' (ID: 456), and 'Inventory Health' (ID: 789). Would you like to see the filters for the sales overview?

---

**👤 You:**
> "Run a query using model 'sales' and view 'orders' for fields 'orders.created_date' and 'orders.total_amount'"

**🤖 AI Agent:**
> Executing inline query… I've retrieved the data from the 'sales' model. For the last 10 orders, the created dates range from yesterday to today, with a total amount of $12,450. Would you like the full 100-row result set?

---

**👤 You:**
> "Find all dashboards related to 'Marketing ROI'"

**🤖 AI Agent:**
> I've searched your content metadata and identified 2 dashboards: 'Global Marketing ROI' (ID: 987) and 'Channel Specific ROI - Beta' (ID: 654). I can fetch the UUIDs and folder paths for either of these.


## Installation & Usage

To install and use the **Looker (Business Intelligence & Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/looker-business-intelligence-data](https://vinkius.com/mcp/looker-business-intelligence-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

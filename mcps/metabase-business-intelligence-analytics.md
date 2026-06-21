# Metabase (Business Intelligence & Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metabase-business-intelligence-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/metabase-business-intelligence-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/metabase-business-intelligence-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Manage your BI environment via Metabase — list dashboards, retrieve visual questions (cards), and search data entities.

## Description
Connect your **Metabase** instance to any AI agent and take full control of your enterprise business intelligence, data visualizations, and reporting through natural conversation.

### What you can do

- **Dashboard Orchestration** — List all managed reporting panels and retrieve detailed layout matrices, including specific card mappings and filter structures directly from your agent
- **Question & Card Audit** — Access visual 'Cards' to retrieve the underlying SQL logic or visualization definitions driving your key business metrics securely
- **Global Content Search** — Execute cross-platform searches to identify Dashboards, Cards, or Data tables matching specific keywords across your entire Metabase instance
- **Collection Navigation** — Explore hierarchical BI Collections (folders) to understand your reporting taxonomy and organizational data boundaries natively
- **Database Inventory** — Enumerate physical data warehouse connections and raw table mappings available for querying within your Metabase environment
- **Metadata Inspection** — Deep-dive into specific Dashboard or Card IDs to retrieve precise JSON representations and chronological data insights instantly

### How it works

1. Subscribe to this server
2. Enter your Metabase Base URL and API Key
3. Start exploring your data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — verify SQL logic and audit dashboard configurations through natural conversation without manual dashboard navigation
- **Business Users** — search for specific reports and retrieve rapid data summaries directly from your workspace
- **Analytics Engineers** — monitor database connections and manage collection hierarchies across multiple Metabase instances efficiently


## Available Tools
- **list_dashboards**: List dashboards mapped in the Metabase BI platform
- **get_dashboard**: Get comprehensive Metabase Dashboard layout matrices
- **list_cards**: Returns heavy lists.

List raw questions (cards) parsed inside Metabase
- **get_card**: Fetch explicit mapping logic behind a specific BI Card
- **list_collections**: List structural BI Collections (folders)
- **list_databases**: List physical Database integrations parsed by Metabase
- **search_content**: Search global reporting entities across Metabase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metabase (Business Intelligence & Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 dashboards created in my Metabase instance"

**🤖 AI Agent:**
> I've retrieved the 5 most recent dashboards. Highlights include 'Q1 Sales Overview' (ID: 123), 'User Engagement Deep-Dive' (ID: 456), and 'Inventory Health' (ID: 789). Would you like to see the cards attached to the sales overview?

---

**👤 You:**
> "Search for any Metabase content related to 'Revenue'"

**🤖 AI Agent:**
> Searching… I've identified several entities: 1) Dashboard 'Annual Revenue Breakdown' (ID: 987), 2) Card 'Monthly Recurring Revenue' (ID: 654), and 3) Table 'public.revenue_events'. Which one would you like to inspect further?

---

**👤 You:**
> "Show me the configuration for card ID '654'"

**🤖 AI Agent:**
> Retrieving card metadata… For 'Monthly Recurring Revenue' (ID: 654), the visualization type is 'Line Chart' and it queries the 'stripe_data' database. The underlying logic uses a filtered aggregation on the 'invoices' table. Would you like to see the full structural JSON?


## Installation & Usage

To install and use the **Metabase (Business Intelligence & Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metabase-business-intelligence-analytics](https://vinkius.com/mcp/metabase-business-intelligence-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

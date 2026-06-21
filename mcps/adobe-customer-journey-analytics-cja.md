# Adobe Customer Journey Analytics (CJA) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adobe-customer-journey-analytics-cja)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/adobe-customer-journey-analytics-cja-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/adobe-customer-journey-analytics-cja-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Omnichannel journey insights — manage data views, connections, and reports via AI.

## Description
Connect your **Adobe Customer Journey Analytics (CJA)** account to your AI agent to unlock professional omnichannel insights and data orchestration. From managing connections to AEP datasets to retrieving complex cross-channel reports and auditing data views, your agent handles your journey analytics ecosystem through natural conversation.

### What you can do

- **Omnichannel Reporting** — Retrieve cross-channel reports that combine web, app, and offline data in a single request
- **Data View Management** — List and audit metadata for data views, including all available dimensions and metrics
- **Connection Oversight** — List and monitor connections between your CJA environment and Adobe Experience Platform datasets
- **Filter Orchestration** — Manage and list filters (formerly segments) to ensure your analysis is targeted and accurate
- **Real-time Journey Tracking** — Quickly identify customer behavior patterns across multiple touchpoints directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adobe Client ID, Client Secret, and IMS Organization ID
3. Start managing your omnichannel analytics and retrieving journey insights through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Omnichannel Analysts** — automate data retrieval across web and offline channels effortlessly
- **CX Managers** — monitor the complete customer journey and identify friction points on the fly
- **Data Engineers** — audit CJA connections and data view configurations using simple commands
- **Product Owners** — retrieve feature engagement data across multiple device platforms instantly


## Available Tools
- **list_data_views**: List CJA data views
- **get_data_view_dimensions**: List dimensions for a data view
- **get_data_view_metrics**: List metrics for a data view
- **get_report**: Retrieve an omnichannel report
- **list_filters**: List journey filters
- **list_connections**: List AEP connections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adobe Customer Journey Analytics (CJA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all data views in my CJA account."

**🤖 AI Agent:**
> I've retrieved your data views. You have 8 active views, including 'Global Web + App', 'Store Transactions', and 'Support Journey'. Which one would you like to explore?

---

**👤 You:**
> "Show me dimensions for data view ID 'dv_12345'."

**🤖 AI Agent:**
> I've retrieved the dimensions for data view 'dv_12345'. You have 120 available dimensions, including 'Page Name', 'Cross-Device ID', and 'Marketing Channel'. Would you like to see the available metrics as well?

---

**👤 You:**
> "List all active filters in my account."

**🤖 AI Agent:**
> I've retrieved your filters. You have 15 active filters, including 'High Value Customers', 'Mobile Sessions', and 'Converted via Email'. Would you like to check the definition for any of them?


## Installation & Usage

To install and use the **Adobe Customer Journey Analytics (CJA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adobe-customer-journey-analytics-cja](https://vinkius.com/mcp/adobe-customer-journey-analytics-cja)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

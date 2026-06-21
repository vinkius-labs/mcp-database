# Clari MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clari)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clari-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clari-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage revenue intelligence and forecasting via Clari — track opportunities, monitor forecasts, and audit pipeline changes directly from any AI agent.

## Description
Connect your **Clari** account to any AI agent and take full control of your revenue operations and forecasting through natural conversation. Streamline how you manage your sales pipeline and historical revenue data.

### What you can do

- **Opportunity Oversight** — List and retrieve details for all CRM opportunities tracked in Clari natively
- **Forecast Intelligence** — Access manual forecast submissions and historical data to understand trends flawlessly
- **Pipeline Auditing** — List and review platform events and audit trail records to track changes securely
- **Account Visibility** — Access CRM accounts associated with revenue data and monitor their status flawlessly
- **User Logistics** — List all users and organization hierarchies to understand team performance securely
- **Export Intelligence** — Monitor the status of asynchronous bulk data export jobs directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clari API Token (obtained from Settings or Clari Support)
3. Start managing your revenue intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Leaders** — monitor forecast accuracy and pipeline health using natural language
- **Revenue Operations** — audit changes to opportunities and monitor export job statuses without opening the dashboard
- **Account Executives** — quickly look up opportunity details and historical forecast values straight from their chat interface
- **Finance Teams** — verify revenue snapshots and fiscal time period configurations


## Available Tools
- **list_clari_users**: List all users and hierarchy in the account
- **get_opportunity_revenue_details**: Get detailed information for a specific opportunity
- **list_revenue_accounts**: List CRM accounts associated with revenue data
- **list_clari_audit_logs**: List platform events and audit trail records
- **list_clari_export_jobs**: List status of asynchronous bulk data export jobs
- **list_clari_forecasts**: List manual forecast submissions and historical data
- **list_revenue_opportunities**: List CRM opportunities tracked in Clari
- **list_clari_time_periods**: List active fiscal years, quarters, and months used in Clari


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clari** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all opportunities worth over $50,000."

**🤖 AI Agent:**
> Retrieving your high-value opportunities... I found 3 deals: 'Acme Enterprise Expansion' ($120k), 'Global Logistics Q3' ($75k), and 'TechCorp Pilot' ($55k). Would you like the full details for the Acme deal?

---

**👤 You:**
> "What is our current manual forecast value?"

**🤖 AI Agent:**
> Checking latest forecast submissions... For the current quarter, the manual aggregate forecast is $2.4M across all regions. This is a 10% increase compared to last week's snapshot.

---

**👤 You:**
> "Who are the account owners for the 'Top 10' pipeline accounts?"

**🤖 AI Agent:**
> Retrieving account ownership data... The Top 10 accounts are managed by: Sarah Miller (4 accounts), Mike Scott (3 accounts), and John Doe (3 accounts).


## Installation & Usage

To install and use the **Clari** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clari](https://vinkius.com/mcp/clari)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

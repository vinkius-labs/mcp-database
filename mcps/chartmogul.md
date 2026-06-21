# ChartMogul MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chartmogul)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chartmogul-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chartmogul-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Analyze subscription revenue and SaaS metrics via ChartMogul — track MRR, churn, and customer growth directly from any AI agent.

## Description
Connect your **ChartMogul** account to any AI agent and take full control of your subscription analytics through natural conversation. Access real-time SaaS metrics like MRR, ARR, and Churn Rate.

### What you can do

- **Metrics Oversight** — Retrieve all high-level subscription metrics (MRR, ARR, ARPA, ASP) natively
- **Growth Intelligence** — Access detailed customer count and churn rate data flawlessly
- **Customer Deep-Dives** — List and retrieve complete profiles for any customer in your database securely
- **Data Logistics** — List and audit all configured data sources providing information to your account flawlessly
- **Revenue Analysis** — Track MRR and ARR trends over specific timeframes directly within your workspace
- **System Verification** — Verify API connectivity and account status using the built-in ping and diagnostic tools

### How it works

1. Subscribe to this server
2. Enter your ChartMogul API Key (obtained from Settings > API Keys)
3. Start querying your SaaS metrics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders & Executives** — monitor business health and revenue growth using natural language
- **Financial Analysts** — audit MRR and ARR trends without manual data exports
- **Customer Success Managers** — quickly look up customer subscription status and history straight from their chat interface
- **Growth Teams** — verify churn rates and customer growth metrics for reporting


## Available Tools
- **get_arr_metrics**: Retrieve Annualized Run Rate metrics
- **get_subscription_metrics**: Retrieve all high-level subscription metrics (MRR, ARR, etc)
- **get_customer_count_metrics**: Retrieve total customer count metrics over time
- **get_mogul_customer_details**: Get detailed information for a specific customer
- **get_mrr_metrics**: Retrieve Monthly Recurring Revenue metrics
- **list_mogul_customers**: List all customers in ChartMogul
- **list_mogul_data_sources**: List all data sources configured in the account
- **ping_mogul_api**: Verify connectivity and authentication with the ChartMogul API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChartMogul** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my total MRR for the last 3 months?"

**🤖 AI Agent:**
> Retrieving MRR data... For the last 3 months, your MRR grew from $45,000 to $52,000, showing a steady upward trend. Would you like to see the breakdown by plan?

---

**👤 You:**
> "Show me details for customer UUID 'cust_123456'."

**🤖 AI Agent:**
> Checking customer 'cust_123456'... This is 'Acme Corp' (john@acme.com). They have been a customer since 2022 and currently have an active 'Enterprise' plan at $1,200/month.

---

**👤 You:**
> "Get my subscription metrics for 2024-01-01 to 2024-03-31."

**🤖 AI Agent:**
> Retrieving metrics for Q1 2024... You ended the quarter with $1.2M ARR, 450 active customers, and a 2.1% net churn rate. I can provide more details on each metric if needed.


## Installation & Usage

To install and use the **ChartMogul** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chartmogul](https://vinkius.com/mcp/chartmogul)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

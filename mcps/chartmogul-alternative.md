# ChartMogul MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chartmogul-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chartmogul-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chartmogul-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Understand your subscription metrics with MRR tracking, churn analysis, and cohort reports that reveal growth opportunities.

## Description
Connect your **ChartMogul** account to any AI agent and take full control of your SaaS revenue intelligence and subscription monitoring workflows through natural conversation.

### What you can do

- **Revenue Orchestration** — Retrieve real-time metrics for Monthly Recurring Revenue (MRR), Annual Run Rate (ARR), and Average Revenue Per Account (ARPA) programmatically
- **Churn & Retention Intelligence** — Monitor customer churn rates and LTV (Lifetime Value) metrics across custom time intervals to understand your business health in real-time
- **Customer Lifecycle Management** — List and manage your subscriber base programmatically, including retrieving detailed historical profiles and MRR contributions
- **Infrastructure Monitoring** — Access information about your connected data sources (Stripe, Braintree, etc.) and subscription plans to ensure high-fidelity billing oversight
- **Trend Analysis** — Query historical metrics over specific periods (day, week, month, quarter) to identify growth patterns and seasonal shifts directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your ChartMogul dashboard (Settings > API)
3. Start managing your SaaS performance from Claude, Cursor, or any MCP client

No more manual scrubbing through filtered charts or exporting CSVs for reporting. Your AI acts as your dedicated SaaS finance analyst and growth coordinator.

### Who is this for?

- **Founders & CEOs** — instantly retrieve high-level revenue summaries and churn reports using natural language commands
- **Finance Teams** — monitor ARR trends and customer LTV without leaving your communication tools
- **Data Analysts** — automate the retrieval of structured SaaS metrics for internal reporting through simple AI queries


## Available Tools
- **create_customer_record**: Add new customer
- **get_summary_metrics**: Get key SaaS metrics
- **get_api_status**: Check connection
- **get_arr_history**: Analyze ARR
- **get_churn_rates**: Analyze retention
- **get_customer_count_history**: Monitor user growth
- **get_customer_details**: Get customer profile
- **get_customer_ltv**: Check Customer LTV
- **get_mrr_history**: Analyze MRR
- **list_customers**: List SaaS customers
- **list_data_sources**: ) connected to ChartMogul.

List connected sources
- **list_subscription_plans**: List billing plans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChartMogul** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show our MRR and ARR summary for the last 3 months."

**🤖 AI Agent:**
> I've retrieved your revenue metrics. Over the last 3 months, your MRR grew by 15%, reaching $54,200. ARR is currently at $650,400. Would you like a breakdown of growth by subscription plan?

---

**👤 You:**
> "What is our current churn rate compared to last month?"

**🤖 AI Agent:**
> Scanning retention metrics... Your current churn rate is 2.4%, down from 2.8% last month. Customer retention is improving. Shall I list the customers who cancelled recently?

---

**👤 You:**
> "Get the MRR contribution for customer 'john.doe@example.com'."

**🤖 AI Agent:**
> Fetching profile... John Doe (ID: uuid_123) contributes $150 to your MRR through a 'Premium Plan'. His LTV is estimated at $4,500 based on his 12-month tenure. Need any other details from his history?


## Installation & Usage

To install and use the **ChartMogul** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chartmogul-alternative](https://vinkius.com/mcp/chartmogul-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

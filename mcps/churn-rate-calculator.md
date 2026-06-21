# Churn Rate Calculator MCP Server

Calculate Customer Churn Rate, Revenue Churn Rate, and Net Revenue Retention (NRR) to instantly assess account health against industry benchmarks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/churn-rate-calculator)

## Overview
**Category:** finance
**Tools Count:** 4

## Description
Finding out why customers leave or why revenue shrinks is critical for business stability. Many companies track raw churn numbers, but they fail to connect lost users to financial impact or account growth momentum. This system solves that by providing a comprehensive view of retention health.

**Mechanism:** The agent connects three core calculations: 1) **Customer Churn Rate (CCR)**, which tracks volume loss using the `customer_churn_rate_calculator` tool; 2) **Revenue Churn Rate (RCR)**, assessing monetary value loss via the `revenue_churn_rate_calculator` tool; and 3) **Net Revenue Retention (NRR)**, incorporating expansion revenue through the `net_revenue_retention_calculator`. Finally, it synthesizes all this data into a clear classification using the `analyze_churn_health` tool.

**Advantage:** Instead of just knowing *that* you lost customers, you know *how much* that loss costs and whether your expansion efforts are enough to offset contraction. The result is an actionable health score (World-Class, Healthy, or Needs Improvement).


## Available Tools
- **analyze_churn_health**: Analyze churn health against industry benchmarks
- **customer_churn_rate_calculator**: Requires start and end customer counts.

Calculate the customer churn rate for a given period
- **net_revenue_retention_calculator**: Requires start ARR, lost revenue, and expansion revenue.

Calculate Net Revenue Retention (NRR) including expansion and contraction
- **revenue_churn_rate_calculator**: Requires start ARR and lost revenue amount.

Calculate the revenue churn rate based on lost ARR


## Installation & Usage

To install and use the **Churn Rate Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/churn-rate-calculator](https://vinkius.com/mcp/churn-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

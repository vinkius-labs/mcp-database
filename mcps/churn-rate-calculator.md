# Churn Rate Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/churn-rate-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/churn-rate-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/churn-rate-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Customer Churn Rate, Revenue Churn Rate, and Net Revenue Retention (NRR) to instantly assess account health against industry benchmarks.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Churn Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I started the year with 1000 customers and ended with 920. My NRR was 1.15, and I operate in the SaaS segment. Analyze our current health."

**🤖 AI Agent:**
> First, let's check the customer volume loss using `customer_churn_rate_calculator` (start: 1000, end: 920). Next, I will use `analyze_churn_health` with the segment 'SaaS', the calculated CCR, and NRR 1.15.

---

**👤 You:**
> "We lost $200k in revenue this quarter, starting from $5M ARR. We gained $350k in upsells. Calculate the NRR and RCR for us."

**🤖 AI Agent:**
> I will calculate the Net Revenue Retention Rate using `net_revenue_retention_calculator` (start: 5000000, lost: 200000, expansion: 350000). I will also run `revenue_churn_rate_calculator` to see the pure financial loss.

---

**👤 You:**
> "What is our current retention status? We have a CCR of 0.12 and an NRR of 0.98, and we are in the ECommerce sector."

**🤖 AI Agent:**
> I will run `analyze_churn_health` for the 'ECommerce' segment using your provided CCR (0.12) and NRR (0.98). Please provide the starting customer count so I can calculate any missing baseline metrics.


## Installation & Usage

To install and use the **Churn Rate Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/churn-rate-calculator](https://vinkius.com/mcp/churn-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

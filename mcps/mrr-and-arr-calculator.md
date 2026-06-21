# MRR and ARR Calculator MCP Server

Calculate Monthly Recurring Revenue (MRR) and Annual Recurring Revenue (ARR) from subscription data, broken down by plan segment.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mrr-and-arr-calculator)

## Overview
**Category:** finance
**Tools Count:** 5

## Description
Building a financial forecast requires more than just total revenue. The challenge is accurately separating the source of growth: where did the money come from? Was it new customers, existing customer upgrades, or was it lost to cancellations?

The MRR and ARR Calculator solves this by providing granular tracking for every component of recurring revenue--New, Expansion, and Churn. It connects raw subscription data (plan price, unit count) to actionable financial metrics.

**Mechanism:** The system uses specialized tools to process your time-series data. First, the `calculate_mrr` tool processes a batch of subscriptions to yield the total MRR for a period. This result is then passed to `aggregate_mrr_components` to separate New, Expansion, and Churn revenue streams. Finally, the `calculate_arr` and `get_metrics_summary` tools take these core metrics to provide annualized forecasts (ARR) and key ratios like ARPU.

**Advantage:** Instead of a single gross number, you get a full financial picture: how fast are you growing (Net New MRR), and what is the true value of your customer base? This allows for precise forecasting and strategic decision-making.


## Available Tools
- **calculate_arr**: Calculate Annual Recurring Revenue from MRR
- **calculate_churn_impact**: Calculate the impact of customer churn on revenue
- **get_metrics_summary**: Get a comprehensive SaaS metrics summary
- **calculate_mrr**: Calculate Monthly Recurring Revenue from subscription data
- **project_revenue**: Project revenue for a given time period


## Installation & Usage

To install and use the **MRR and ARR Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mrr-and-arr-calculator](https://vinkius.com/mcp/mrr-and-arr-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

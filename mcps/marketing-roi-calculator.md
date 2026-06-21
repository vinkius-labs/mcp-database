# Marketing ROI Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketing-roi-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/marketing-roi-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/marketing-roi-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate marketing Return on Investment (ROI), payback period, and efficiency across all campaigns using detailed cost and revenue attribution.

## Description
Are you struggling to prove the true value of your marketing spend? Many teams calculate ROI based only on last-click metrics, missing crucial operational costs and complex customer journeys. This system solves that problem by providing a comprehensive financial analysis framework.

**The Mechanism:** The Marketing ROI Calculator connects detailed cost data with attributed revenue using advanced models. First, you use the `query_marketing_investment_total` tool to aggregate all spending--including media spend, production costs, headcount overhead, and tools expense--into one verified total investment figure. Next, the `calculate_attributed_revenue` tool applies sophisticated attribution logic (like Time-Decay) to raw revenue data, ensuring credit is given correctly across the entire customer journey. Finally, the `compute_rois_metrics_comparative` tool synthesizes these inputs, delivering a full dashboard of ROI percentage, payback months, and efficiency metrics for side-by-side comparison.

**The Advantage:** Stop guessing your marketing performance. Gain deterministic, auditable financial insights that show exactly which campaigns deliver the highest true profit relative to their total investment.


## Available Tools
- **compute_rois_metrics_comparative**: Compute ROI metrics and compare performance across multiple campaigns
- **query_marketing_investment_total**: Calculate total marketing investment for a campaign within a date range
- **calculate_attributed_revenue**: Calculate attributed gross revenue for a campaign using an attribution model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketing ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to compare Q1's performance for three campaigns: 'Spring2024_Launch', 'SEO Blitz', and 'Content Drive'. The gross margin is 0.65. Please run the full ROI comparison."

**🤖 AI Agent:**
> First, I will aggregate costs using `query_marketing_investment_total` for each campaign's period. Then, I will calculate attributed revenue via `calculate_attributed_revenue`. Finally, I pass all results to `compute_rois_metrics_comparative` with the gross margin of 0.65.

---

**👤 You:**
> "Calculate the total investment for 'SummerSale' from 2024-06-01 to 2024-08-31. Media spend was $50k, production was $10k, headcount overhead was $15k, and tools were $5k."

**🤖 AI Agent:**
> I will call `query_marketing_investment_total` with the following parameters: campaignId='SummerSale', startDate='2024-06-01', endDate='2024-08-31', mediaSpend=50000, productionCost=10000, headcountOverhead=15000, toolsExpense=5000. This gives the total investment needed for attribution.

---

**👤 You:**
> "Using a TIME_DECAY model, find the attributed revenue and conversion count for 'Spring2024_Launch' from 2024-01-01 to 2024-03-31. Raw revenue was $500k with 100 conversions."

**🤖 AI Agent:**
> I will use the `calculate_attributed_revenue` tool, specifying campaignId='Spring2024_Launch', reportingPeriodStartDate='2024-01-01', reportingPeriodEndDate='2024-03-31', attributionModelType='TIME_DECAY', rawRevenue=500000, and conversionCount=100. This gives the most accurate gross revenue figure.


## Installation & Usage

To install and use the **Marketing ROI Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketing-roi-calculator](https://vinkius.com/mcp/marketing-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

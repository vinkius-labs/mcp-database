# LTV:CAC Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ltvcac-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ltvcac-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ltvcac-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine if your customer acquisition strategy is profitable by calculating LTV, CAC, and the critical LTV:CAC ratio.

## Description
# Assess Unit Economics with Precision

The challenge for any growing business is knowing if spending money to acquire a customer actually generates profit. Many companies struggle to connect their marketing spend (CAC) directly to the long-term value of that customer (LTV). This gap in understanding leads to inefficient spending and unsustainable growth projections.

Our MCP provides a clear mechanism to bridge this financial intelligence gap. It guides users through three core calculations:

1. **Projecting Lifetime Value:** Using `calculate_ltv`, you input the Average Revenue Per User (ARPU), gross margin, and churn rate to forecast the total value of a customer over time.
2. **Pinpointing Acquisition Cost:** With `calculate_cac`, you provide detailed spend data across different channels. The tool computes the precise cost required to acquire one paying user from each source.
3. **Evaluating Profitability:** Finally, `evaluate_profitability` synthesizes these two metrics with your gross margin and time period to deliver the LTV:CAC ratio, a payback period in months, and a clear verdict (Optimal, Warning, or Critical).

The result is not just a number; it's an actionable measure of financial health. You can immediately determine if your marketing spend supports sustainable growth.


## Available Tools
- **calculate_cac**: Accepts JSON array of {channelName, totalSpend, newCustomersAcquired} objects.

Calculate Customer Acquisition Cost (CAC) per marketing channel
- **calculate_ltv**: LTV = ARPU × (1 / churnRate) × grossMarginPercentage.

Calculate Customer Lifetime Value (LTV) based on ARPU, gross margin, and churn rate
- **evaluate_profitability**: Evaluate LTV:CAC ratio, payback period, and profitability verdict


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LTV:CAC Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My ARPU is $1200, gross margin is 0.65 (65%), and my annual churn rate is 0.08 (8%). Please calculate the LTV."

**🤖 AI Agent:**
> I will first run `calculate_ltv` with ARPU=1200, grossMarginPercentage=0.65, and churnRateAnnualPct=0.08. The projected LTV is $10,533.33.

---

**👤 You:**
> "Calculate CAC for these two channels: Paid Search ($20k spend, 40 customers) and Organic Content ($5k spend, 100 customers)."

**🤖 AI Agent:**
> Using `calculate_cac`, the resulting CAC is $0.50 for Paid Search ($20k/40) and $0.05 for Organic Content ($5k/100). Total CAC is $10,500.

---

**👤 You:**
> "Given an LTV of $10,533.33 and a total CAC of $10,500, with a gross margin of 0.65 over 12 months, what is the profitability verdict?"

**🤖 AI Agent:**
> I will run `evaluate_profitability` using LTV=$10533.33, totalCacAmount=$10500, grossMarginPercentage=0.65, and timePeriodMonths=12. The result shows an Optimal verdict (ratio > 5:1).


## Installation & Usage

To install and use the **LTV:CAC Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltvcac-calculator](https://vinkius.com/mcp/ltvcac-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

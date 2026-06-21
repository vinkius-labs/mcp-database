# LTV:CAC Calculator MCP Server

Determine if your customer acquisition strategy is profitable by calculating LTV, CAC, and the critical LTV:CAC ratio.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ltvcac-calculator)

## Overview
**Category:** finance
**Tools Count:** 3

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


## Installation & Usage

To install and use the **LTV:CAC Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltvcac-calculator](https://vinkius.com/mcp/ltvcac-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

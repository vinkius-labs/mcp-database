# Growth Rate Calculator MCP Server

Calculate MoM, QoQ, YoY growth rates and model multi-scenario financial projections (CAGR, Rule of 40) from historical revenue data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/growth-rate-calculator)

## Overview
**Category:** finance
**Tools Count:** 3

## Description
# Assess Growth Trajectory with Financial Precision

The core challenge for any growing business is quantifying performance over time. Simply looking at last month's revenue is insufficient; true financial health requires comparing current results against historical benchmarks (like the same quarter last year) and projecting future potential under different growth assumptions.

This MCP provides a systematic way to analyze sequential financial data, moving beyond simple arithmetic averages to provide actionable metrics: directional momentum (MoM/QoQ), long-term stability (YoY/CAGR), and operational efficiency (Rule of 40).

## How the System Works (The Mechanism)

The server operates through three connected tools that model different aspects of financial performance:

1. **Analyzing Directional Momentum:** Use `analyze_historical_growth` to instantly calculate Month-over-Month, Quarter-over-Quarter, and Year-over-Year growth rates across your entire dataset. This identifies immediate trends and volatility.
2. **Synthesizing Core Benchmarks:** Next, run `calculate_key_rates`. By feeding the historical revenue and EBITDA data, this tool computes two critical benchmarks: the Compound Annual Growth Rate (CAGR) for overall sustained growth, and the Rule of 40 score, which combines your growth rate with profitability.
3. **Forecasting Future Potential:** Finally, use `generate_growth_projection`. This tool takes the most recent revenue figure and projects a full twelve months into the future, allowing you to model 'Constant', 'Accelerated', or 'Decelerated' scenarios based on your expected market shifts.

The result is not just a set of numbers; it is a comprehensive financial blueprint that helps determine if your growth rates are sustainable, profitable, and where your business stands relative to key industry benchmarks.


## Available Tools
- **analyze_historical_growth**: Pass data as a JSON array of objects with date and revenue fields.

Analyze historical revenue growth across time periods
- **calculate_key_rates**: Pass EBITDA metrics as a JSON array of {revenue, ebitda} objects.

Calculate CAGR and Rule of 40 score from financial data
- **generate_growth_projection**: For Accelerated/Decelerated, provide rateDeterminer as the monthly rate shift percentage.

Generate 12-month revenue projections under different growth scenarios


## Installation & Usage

To install and use the **Growth Rate Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growth-rate-calculator](https://vinkius.com/mcp/growth-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

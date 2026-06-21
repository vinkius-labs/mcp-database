# Influencer ROI Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/influencer-roi-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/influencer-roi-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/influencer-roi-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate the financial impact, EMV, and profitability of influencer marketing campaigns.

## Description
This MCP server provides specialized analytical tools to quantify the media value and economic efficiency of influencer partnerships. Use `get_engagement_valuation` to determine Earned Media Value (EMV) and Cost Per Engagement (CPE). Use `get_conversion_economics` to analyze campaign profitability, including estimated conversions, CPA, and projected lifetime revenue based on LTV. You can also use `compare_to_paid_social` to evaluate how influencer performance compares against standard paid social benchmarks.


## Available Tools
- **get_engagement_valuation**: Determines the media value and engagement efficiency of a campaign
- **compare_to_paid_social**: Compares influencer campaign efficiency to paid social benchmarks
- **get_conversion_economics**: Analyzes campaign profitability based on conversions and customer value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Influencer ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the EMV for an influencer campaign that cost $500, reached 50,000 people, had a 5% engagement rate, and a CPM benchmark of $10."

**🤖 AI Agent:**
> The `get_engagement_valuation` tool would return an Earned Media Value (EMV) of $500 and a Cost Per Engagement (CPE) of $0.20.

---

**👤 You:**
> "Analyze the profitability of an influencer campaign with $1000 cost, 10,000 reach, 2% engagement rate, 1% conversion rate, and $50 LTV."

**🤖 AI Agent:**
> The `get_conversion_economics` tool would return 2 estimated conversions, a CPA of $500, projected lifetime revenue of $100, and an ROI of -90%.

---

**👤 You:**
> "Compare an influencer CPA of $5 to a paid social benchmark CPA of $8."

**🤖 AI Agent:**
> The `compare_to_paid_social` tool would show an efficiency delta of 37.5% and a performance status of 'Outperforming'.


## Installation & Usage

To install and use the **Influencer ROI Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/influencer-roi-calculator](https://vinkius.com/mcp/influencer-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

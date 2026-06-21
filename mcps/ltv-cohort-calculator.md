# LTV Cohort Calculator MCP Server

Calculate Customer Lifetime Value (LTV) for any acquisition cohort, projecting future revenue trends.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ltv-cohort-calculator)

## Overview
**Category:** data-analytics
**Tools Count:** 3

## Description
**[Hook]** Understanding the true value of a customer group is critical to sustainable business growth. But raw revenue data doesn't tell the full story.


## Available Tools
- **calculate_cumulative_ltv**: Milestones are specified as months after acquisition.

Calculate total accumulated LTV at fixed milestones for a cohort
- **fetch_cohort_metrics**: Use acquireMonth in YYYY-MM format and optionally specify how many months of history to retrieve.

Fetch raw accumulated monthly revenues for a given acquisition cohort
- **generate_ltv_projections**: Historical metrics must be provided as a JSON array of objects with periodIndex and accumulatedRevenueValue fields.

Project LTV at 36 months using linear and logarithmic extrapolation methods


## Installation & Usage

To install and use the **LTV Cohort Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltv-cohort-calculator](https://vinkius.com/mcp/ltv-cohort-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

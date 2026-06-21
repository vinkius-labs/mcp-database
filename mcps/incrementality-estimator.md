# Incrementality Estimator MCP Server

Determines true campaign ROI by calculating lift above natural conversion rates using control group data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/incrementality-estimator)

## Overview
**Category:** analytics
**Tools Count:** 3

## Description
# Quantify True Campaign Impact

The marketing industry often uses standard Return on Ad Spend (ROAS), which calculates return based only on the exposed group. This method is flawed because it treats all conversions as incremental, ignoring the natural conversion rate that would have occurred anyway--the baseline.

**The Problem:** Simple ROAS inflates perceived value by mixing true campaign impact with organic activity.

**The Mechanism (How it works):** The Incrementality Estimator solves this by establishing a statistically sound comparison. We first use the `calculate_baseline_metrics` tool to determine the natural conversion rate from an untreated control group. Then, we pass these baselines into `calculate_incrementality_metrics`, which isolates the absolute and percentage lift attributable *only* to the campaign treatment. Finally, `calculate_roas_comparison` converts this incremental volume into a true Return on Ad Spend (ROAS), giving you a marginal return figure that is actionable.

**The Advantage:** You move beyond simple reporting to quantify the exact monetary value of your intervention, ensuring budget allocation decisions are based on proven lift, not inflated metrics.


## Available Tools
- **calculate_baseline_metrics**: Required before any lift calculation can begin.

Calculate baseline conversion rates for control and exposed groups
- **calculate_incrementality_metrics**: Determines how much better the exposed campaign performed versus what would have happened without it.

Calculate incrementality metrics including absolute lift, percentage lift, and incremental CPA
- **calculate_roas_comparison**: Calculate true incremental ROAS and compare it to reported channel ROAS


## Installation & Usage

To install and use the **Incrementality Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incrementality-estimator](https://vinkius.com/mcp/incrementality-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

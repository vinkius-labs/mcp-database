# Incrementality Estimator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/incrementality-estimator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/incrementality-estimator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/incrementality-estimator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Determines true campaign ROI by calculating lift above natural conversion rates using control group data.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incrementality Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We ran a campaign for $10,000. The exposed group had 500 users (20 conversions), and the control group had 400 users (8 conversions). What is our true lift?"

**🤖 AI Agent:**
> First, run `calculate_baseline_metrics` with exposed group size=500, exposed conversions=20, control group size=400, and control conversions=8. Next, use `calculate_incrementality_metrics` to find the absolute lift. Finally, if average conversion value is $50, run `calculate_roas_comparison` to get the true ROAS.

---

**👤 You:**
> "Given a baseline CR of 3% and an exposed group size of 10,000 with a total cost of $20,000. Calculate the estimated incremental conversions and resulting CPA."

**🤖 AI Agent:**
> I will use `calculate_incrementality_metrics` first to determine the absolute lift volume based on the 3% baseline. Then, I can pass that incremental volume and the $20,000 cost into `calculate_roas_comparison` to see how profitable our true return is.

---

**👤 You:**
> "Our total campaign spend was $5,000. We identified 120 truly incremental conversions with an average value of $75 each. What is the true ROAS?"

**🤖 AI Agent:**
> I will use `calculate_roas_comparison` directly. I need to input incremental conversions=120, total campaign cost=$5,000, and average conversion value=$75. This gives us the most accurate profitability metric.


## Installation & Usage

To install and use the **Incrementality Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incrementality-estimator](https://vinkius.com/mcp/incrementality-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

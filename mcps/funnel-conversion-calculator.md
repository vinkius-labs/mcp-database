# Funnel Conversion Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funnel-conversion-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/funnel-conversion-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/funnel-conversion-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-analytics](../categories/marketing-analytics.md)

Calculate marketing funnel metrics step-by-step and project revenue gains from process improvements.

## Description
Connect this Funnel Conversion Calculator to any AI agent. The funnel is a critical path: Awareness $\to$ Consideration $\to$ Intent $\to$ Purchase. If you don't know where the leaks are, optimizing anything is wasted effort.

**Mechanism:** This toolset provides three core functions:
1. **`calculate_funnel_metrics`**: Establishes your baseline performance by calculating current conversion rates and projected revenue from a starting volume.
2. **`identify_bottleneck`**: Analyzes the baseline results to pinpoint the exact stage (e.g., Consideration) where drop-offs are most severe relative to potential volume, showing you where effort matters most.
3. **`simulate_improvement_impact`**: Allows you to run 'what-if' scenarios. By proposing percentage lifts in specific conversion rates, this function models the resulting additional purchases and the total monetary uplift (projected revenue gain). 

The bridge this provides is direct: It connects raw marketing data volume into actionable financial projections, telling your team exactly how much more money a 1% improvement at the Consideration stage could generate.


## Available Tools
- **identify_bottleneck**: Returns the bottleneck stage name, relative loss percentage, and improvement leverage calculation.

Identify the funnel stage with the highest relative drop-off rate
- **calculate_funnel_metrics**: Calculate funnel conversion metrics across Awareness, Consideration, Intent, and Purchase stages
- **simulate_improvement_impact**: Returns recalculated metrics, overall improvement percentage, additional purchases, and revenue uplift.

Simulate projected financial uplift from targeted funnel stage improvements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Funnel Conversion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the initial analysis. Start with 10,000 leads and assume A->C is 25%, C->I is 30%, and I->P is 70%. The average customer value is $150."

**🤖 AI Agent:**
> The `calculate_funnel_metrics` tool shows a baseline revenue of $3,150. The bottleneck appears to be Consideration, which has the highest relative drop-off.

---

**👤 You:**
> "I want to model an improvement. Let's assume we can improve Consideration by 10% (30% -> 33%) and Intent by 5% (70% -> 73%). Recalculate the impact."

**🤖 AI Agent:**
> Using `simulate_improvement_impact`, we project that these targeted improvements increase total purchases by 450 units, resulting in a $67,500 projected revenue uplift.

---

**👤 You:**
> "Identify the bottleneck for this quarter's data snapshot (A->C: 20%, C->I: 40%, I->P: 65%). Initial volume was 8,000. ARPC is $140."

**🤖 AI Agent:**
> The `identify_bottleneck` tool confirms that the Consideration stage presents the highest relative loss point, requiring immediate focus to maximize return on investment.


## Installation & Usage

To install and use the **Funnel Conversion Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funnel-conversion-calculator](https://vinkius.com/mcp/funnel-conversion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

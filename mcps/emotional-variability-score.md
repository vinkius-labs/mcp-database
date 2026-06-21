# Emotional Variability Score MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emotional-variability-score)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emotional-variability-score-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emotional-variability-score-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify emotional fluctuations, mood amplitude, and longitudinal stability.

## Description
This MCP server provides specialized tools to analyze emotional patterns over time. Use `calculate_instability_index` to quantify the frequency of mood swings, or `calculate_mood_amplitude` to identify the extremes between peak and valley states. You can also use `compare_weekly_volatility` to track changes in stability week-over-week, or `get_comprehensive_emotional_report` for a high-level summary of emotional metrics.


## Available Tools
- **compare_weekly_volatility**: Returns delta and trend.

Determine if emotional instability is worsening or improving by comparing two consecutive weeks
- **calculate_mood_amplitude**: Returns peak, valley, and total range.

Identify the extremes of the emotional range experienced during a period
- **calculate_instability_index**: Returns instability score and pattern type.

Quantify how erratic or frequent the mood swings are within a specific date range
- **get_comprehensive_emotional_report**: Returns aggregated stability status, range, and rating.

Generate a high-level summary of all emotional metrics for a given period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emotional Variability Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the instability index for the period between 2023-10-01 and 2023-10-07."

**🤖 AI Agent:**
> The `calculate_instability_index` tool would return the instability score and pattern type for that specific week.

---

**👤 You:**
> "What was the peak and valley mood score between 2023-10-01 and 2023-10-31?"

**🤖 AI Agent:**
> The `calculate_mood_amplitude` tool would return the peak value, valley value, and the total range scale for October.

---

**👤 You:**
> "Generate an emotional report for the first week of November 2023."

**🤖 AI Agent:**
> The `get_comprehensive_emotional_report` tool would provide a summary including instability status, amplitude range, and an overall stability rating.


## Installation & Usage

To install and use the **Emotional Variability Score** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emotional-variability-score](https://vinkius.com/mcp/emotional-variability-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

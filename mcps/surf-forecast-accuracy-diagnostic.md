# Surf Forecast Accuracy Diagnostic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-forecast-accuracy-diagnostic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Evaluate surf forecast precision by comparing predicted wave conditions against real-world observations.

## Description
This MCP server provides diagnostic tools to evaluate the precision of surf forecast models. By comparing predicted wave conditions against real-world observations, it enables optimized model selection and bias adjustment. Use `get_model_performance_stats` to retrieve reliability scores, `calculate_bias_correction` to find adjustment factors for metrics like wave height, and `recommend_best_model` to identify the most trustworthy forecast for specific sea states and regions. It also includes `verify_forecast_integrity` to ensure historical data is sufficient for analysis.


## Available Tools (4)
- **calculate_bias_correction**: Calculate the bias correction factor for a model variable
- **get_model_performance_stats**: Get accuracy statistics for a specific model in a region over a time range
- **recommend_best_model**: Recommend the most reliable model for a region and condition
- **verify_forecast_integrity**: Verify the integrity of historical forecast data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Forecast Accuracy Diagnostic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How accurate has the 'global_swell_v2' model been in the North Atlantic over the last month?"

**🤖 AI Agent:**
> The 'global_swell_v2' model has an accuracy score of 0.88 and a High reliability rating in the North Atlantic for the requested period.

---

**👤 You:**
> "Which model should I trust most for wind chop in the South Pacific?"

**🤖 AI Agent:**
> The 'regional_pacific_pro' model is recommended for wind chop in the South Pacific with an expected accuracy of 0.92.

---

**👤 You:**
> "How much should I adjust the wave height predictions for the 'ocean_master' model in the North Atlantic?"

**🤖 AI Agent:**
> The correction factor for waveHeight for the 'ocean_master' model in the North Atlantic is 1.05, with a confidence level of 0.94.


## ❓ FAQ

**Q: How can I find the most reliable model for swell conditions?**
You can use the `recommend_best_model` tool, specifying the region and setting the condition type to 'swell'.

**Q: What is a bias correction factor?**
It is a multiplier used to adjust model predictions to better match observed reality, calculated via `calculate_bias_correction`.

**Q: Can I check if there is enough data for a specific region?**
Yes, use `verify_forecast_integrity` to check data completeness and whether the volume is sufficient for statistical analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-forecast-accuracy-diagnostic](https://vinkius.com/en/ai-agent-connect/surf-forecast-accuracy-diagnostic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Forecast Accuracy Diagnostic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-forecast-accuracy-diagnostic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Forecast Accuracy Diagnostic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-forecast-accuracy-diagnostic": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

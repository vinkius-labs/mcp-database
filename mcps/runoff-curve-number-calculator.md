# Runoff Curve Number Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/runoff-curve-number-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Calculate surface runoff using the SCS Curve Number method.

## Description
This MCP server provides tools to estimate surface runoff using the Soil Conservation Service (SCS) Curve Number method. It allows users to determine base curve numbers based on land use and soil groups, adjust those numbers for different Antecedent Moisture Conditions (AMC), and calculate runoff depth and volume for specific rainfall events. Use `get_base_curve_number` to find the initial CN, `calculate_adjusted_cn` to account for soil wetness, and `calculate_runoff_depth` to find the final runoff amount.


## Available Tools (5)
- **calculate_runoff_depth**: Calculates the depth of water that will run off given a specific rainfall event
- **calculate_adjusted_cn**: Adjusts the base Curve Number based on the current Antecedent Moisture Condition
- **calculate_runoff_parameters**: Calculates the physical runoff potential constants (Potential Maximum Retention and Initial Abstraction) for a specific CN
- **generate_storm_series_runoff**: Predicts runoff depth for a sequence of different storm events for a single landscape
- **get_base_curve_number**: Determines the standard Curve Number for a specific land use and soil group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runoff Curve Number Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the base curve number for forest land in soil group A?"

**🤖 AI Agent:**
> The base curve number for forest land in soil group A is 30.

---

**👤 You:**
> "Calculate the runoff depth for 50mm of rain with a CN of 75 and initial abstraction of 5mm."

**🤖 AI Agent:**
> The runoff depth for 50mm of rainfall is 33.33mm.

---

**👤 You:**
> "Adjust a base CN of 80 for AMC III conditions."

**🤖 AI Agent:**
> The adjusted curve number for AMC III is 91.2.


## ❓ FAQ

**Q: What is the SCS Curve Number method?**
It is an empirical model used to estimate direct runoff from precipitation in small watersheds based on soil type and land cover.

**Q: How do I account for wet soil conditions?**
You can use the `calculate_adjusted_cn` tool to adjust the base Curve Number for AMC I (dry), AMC II (average), or AMC III (wet) conditions.

**Q: Can I calculate runoff for multiple storm events at once?**
Yes, the `generate_storm_series_runoff` tool allows you to provide a list of rainfall depths to predict a series of runoff results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/runoff-curve-number-calculator](https://vinkius.com/ai-agent-connect/runoff-curve-number-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runoff Curve Number Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runoff-curve-number-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runoff Curve Number Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runoff-curve-number-calculator": {
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

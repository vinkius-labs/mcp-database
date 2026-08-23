# Continuous Glucose Trend Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/continuous-glucose-trend-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Predictive CGM glucose velocity and trend arrow analysis.

## Description
This MCP server provides deterministic predictive analysis for Continuous Glucose Monitor (CGM) data. It calculates glucose velocity (rate of change), identifies visual trend arrows, and predicts future glucose levels. Use `calculate_glucose_trends` to determine the direction of glucose movement and receive proactive safety actions if rapid drops are detected. It also includes `validate_glucose_readings` to ensure data consistency and `get_velocity_threshold_definitions` to understand the velocity boundaries used for trend classification.


## Available Tools (3)
- **calculate_glucose_trends**: Calculates the velocity, visual trend symbol, and future glucose prediction based on a window of historical readings
- **get_velocity_threshold_definitions**: Retrieves the boundary values for all trend arrow classifications
- **validate_glucose_readings**: Ensures the provided glucose history is chronologically consistent and physically possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Continuous Glucose Trend Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these glucose readings: current 90, 15 mins ago 110, 30 mins ago 130."

**🤖 AI Agent:**
> The rate of change is -1.33 mg/dL/min. The trend is 'Diagonal Down'. The predicted glucose in 30 minutes is 40 mg/dL. Proactive action: none.

---

**👤 You:**
> "What is the trend if my current glucose is 80 and 30 minutes ago it was 180?"

**🤖 AI Agent:**
> The rate of change is -3.33 mg/dL/min. The trend is 'Double Down'. The predicted glucose in 30 minutes is -20 mg/dL. Proactive action: consume 15g carbs immediately.

---

**👤 You:**
> "Check the trend for current 150, 15 mins ago 145, 30 mins ago 140."

**🤖 AI Agent:**
> The rate of change is 0.33 mg/dL/min. The trend is 'Flat'. The predicted glucose in 30 minutes is 160 mg/dL. Proactive action: none.


## ❓ FAQ

**Q: How does the trend arrow prediction work?**
The tool calculates the rate of change by comparing the current glucose reading with the reading from 30 minutes ago. This velocity is then used to assign a trend arrow like 'Double Up' or 'Double Down'.

**Q: What is a proactive action?**
A proactive action is a safety recommendation. For example, if `calculate_glucose_trends` detects a 'Double Down' trend while glucose is below 100 mg/dL, it will recommend consuming 15g of carbs immediately.

**Q: Can I validate my CGM data?**
Yes, you can use the `validate_glucose_readings` tool to check if your glucose history is chronologically consistent and physically possible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/continuous-glucose-trend-calculator](https://vinkius.com/ai-agent-connect/continuous-glucose-trend-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Continuous Glucose Trend Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `continuous-glucose-trend-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Continuous Glucose Trend Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "continuous-glucose-trend-calculator": {
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

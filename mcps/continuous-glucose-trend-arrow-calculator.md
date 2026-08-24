# Continuous Glucose Trend Arrow Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/continuous-glucose-trend-arrow-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Predictive CGM velocity and trend arrow analysis.

## Description
This MCP server provides deterministic predictive analysis for Continuous Glucose Monitor (CGM) data. It calculates glucose velocity, visual trend arrows, and predicted glucose levels. Users can utilize `get_glucose_velocity_analysis` for a full breakdown of rate of change and predicted values, `get_trend_status` for quick visual direction, or `get_proactive_intervention_alert` to identify immediate hypoglycemia risks.


## Available Tools (3)
- **get_glucose_velocity_analysis**: Calculates the precise rate of change, the visual trend arrow, and the predicted glucose level
- **get_proactive_intervention_alert**: Determines if an immediate corrective action is required to prevent hypoglycemia
- **get_trend_status**: Returns only the visual trend classification for a user to quickly interpret direction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Continuous Glucose Trend Arrow Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my glucose: current is 90, 15 mins ago was 100, and 30 mins ago was 120."

**🤖 AI Agent:**
> Rate of change: -1.0 mg/dL/min. Trend: Diagonal Down. Predicted BG in 30 mins: 60 mg/dL. Proactive action: consume 15g carbs immediately.

---

**👤 You:**
> "What is my current glucose trend? Current is 150, 30 mins ago was 140."

**🤖 AI Agent:**
> Your trend is Diagonal Up.

---

**👤 You:**
> "Check if I need to take action. Current is 110, 30 mins ago was 130."

**🤖 AI Agent:**
> No immediate action is required.


## ❓ FAQ

**Q: What does the trend arrow represent?**
The trend arrow represents the velocity of your glucose change, indicating how fast your levels are rising or falling.

**Q: How is the predicted glucose calculated?**
It is calculated by taking the current glucose level and adding the change expected over the next 30 minutes based on current velocity.

**Q: When is a proactive action recommended?**
A proactive action like consuming carbohydrates is recommended when a 'Double Down' trend is detected while glucose is below 100 mg/dL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/continuous-glucose-trend-arrow-calculator](https://vinkius.com/ai-agent-connect/continuous-glucose-trend-arrow-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Continuous Glucose Trend Arrow Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `continuous-glucose-trend-arrow-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Continuous Glucose Trend Arrow Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "continuous-glucose-trend-arrow-calculator": {
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

# Cycling Power to Speed Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cycling-power-to-speed-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Converts cycling power output into estimated speed and performance metrics.

## Description
This MCP server provides a physics-based engine to translate cycling power into real-world performance expectations. By accounting for rider weight, bike weight, terrain grade, and wind conditions, it calculates precise metrics. Use `get_estimated_speed` to predict velocity, `get_energy_expenditure` to track kilojoules, `get_time_to_distance` to plan routes, and `get_power_to_weight_metrics` to analyze efficiency.


## Available Tools (4)
- **get_energy_expenditure**: Determines the total energy consumed during a specific duration of effort
- **get_estimated_speed**: Calculates the expected velocity for a given power output and environmental context
- **get_power_to_weight_metrics**: Provides a breakdown of the power-to-weight efficiency for a specific setup
- **get_time_to_distance**: Predicts how long it will take to cover a specific distance at a given power level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling Power to Speed Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my estimated speed if I ride at 250 watts with a 75kg rider, 10kg bike, on a 3% grade with a 10km/h headwind?"

**🤖 AI Agent:**
> Your estimated speed is 32.4 km/h.

---

**👤 You:**
> "How much energy will I spend riding at 200 watts for 30 minutes?"

**🤖 AI Agent:**
> You will expend 60.0 kilojoules.

---

**👤 You:**
> "How long will it take to cover 20km at 200 watts on flat ground with no wind, given a 70kg rider and 8kg bike?"

**🤖 AI Agent:**
> It will take approximately 35 minutes and 12 seconds to cover 20km.


## ❓ FAQ

**Q: How does the speed estimation work?**
The engine calculates speed by modeling gravity resistance, rolling resistance, and aerodynamic drag based on your power and environmental inputs.

**Q: Can I account for wind direction?**
Yes, you can specify headwind, tailwind, or crosswind to get an accurate speed estimate.

**Q: What metrics are provided?**
The server provides estimated speed, power-to-weight ratio, energy expenditure in kilojoules, and travel time for specific distances.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cycling-power-to-speed-estimator](https://vinkius.com/en/ai-agent-connect/cycling-power-to-speed-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling Power to Speed Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-power-to-speed-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling Power to Speed Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-power-to-speed-estimator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

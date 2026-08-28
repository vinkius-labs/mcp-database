# Spray Drift Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spray-drift-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Estimates pesticide drift distance and risk using agdrift equations.

## Description
This MCP server provides precise pesticide movement simulations. It uses the agdrift model to calculate droplet deposition, evaporation effects, and canopy interception. Use `calculate_drift_dynamics` to model droplet behavior, `estimate_canopy_impact` to adjust for foliage density, `evaluate_drift_risk` to classify danger levels, and `determine_buffer_zone` to establish safe distances for non-target areas.


## Available Tools (4)
- **calculate_drift_dynamics**: Determine the physical behavior and movement of droplets based on spray and environmental parameters
- **estimate_canopy_impact**: Adjust drift predictions based on the presence and density of a target crop
- **evaluate_drift_risk**: Categorize the level of danger posed by the current application parameters
- **determine_buffer_zone**: Calculate the minimum safe distance required to protect non-target areas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spray Drift Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the drift dynamics for a fine droplet size with 5 m/s wind speed, 2m boom height, 100 L/ha rate, 25C, and 50% humidity."

**🤖 AI Agent:**
> The calculated deposition at 10m is 0.045 and at 20m is 0.012, with an evaporation factor of 1.15.

---

**👤 You:**
> "What is the required buffer zone for a High risk level with 4 m/s wind speed and Medium droplets?"

**🤖 AI Agent:**
> The required buffer distance is 35 meters.

---

**👤 You:**
> "Evaluate the drift risk for a deposition of 0.05 at a target with an application rate of 150 L/ha."

**🤖 AI Agent:**
> The risk level is Moderate with a risk score of 0.65.


## ❓ FAQ

**Q: How accurate are the drift predictions?**
Predictions are based on the agdrift model equations, accounting for wind, droplet size, and environmental factors like humidity and temperature.

**Q: Can I calculate the required safety distance?**
Yes, use the `determine_buffer_zone` tool to calculate the minimum safe distance based on wind speed and risk level.

**Q: Does the model account for crop density?**
Yes, the `estimate_canopy_impact` tool allows you to adjust deposition based on the density of the target crop canopy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spray-drift-model](https://vinkius.com/ai-agent-connect/spray-drift-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spray Drift Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spray-drift-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spray Drift Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spray-drift-model": {
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

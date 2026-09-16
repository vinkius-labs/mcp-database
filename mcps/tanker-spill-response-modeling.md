# Tanker Spill Response Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tanker-spill-response-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Models oil spill trajectory, weathering, and shoreline impact.

## Description
This MCP server provides specialized tools for modeling the movement and environmental fate of oil spills. It allows AI agents to predict the path of a spill using `get_spill_trajectory`, determine the physical state of the oil through `calculate_weathering_state`, estimate when oil will reach land with `predict_shoreline_impact`, and evaluate environmental threats using `get_spill_risk_assessment`.


## Available Tools (4)
- **calculate_weathering_state**: Determines the physical state and remaining volume of the oil at a specific time
- **get_spill_risk_assessment**: Provides a high-level summary of the environmental threat based on the current spill status
- **get_spill_trajectory**: Predicts the movement path of the oil slick over a specific duration
- **predict_shoreline_impact**: Estimates when and where the oil will strike a coastline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tanker Spill Response Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the movement of a 500 cubic meter oil spill starting at latitude -34.0 and longitude 18.0, with wind at 5 m/s at 90 degrees, current at 0.5 m/s at 180 degrees, for 24 hours."

**🤖 AI Agent:**
> The oil spill is predicted to move south-southeast, covering a total distance of 12.4 kilometers over 24 hours, with the center of mass reaching coordinates -34.12, 18.05.

---

**👤 You:**
> "What is the weathering state of 450 cubic meters of oil after 48 hours, given an oil density of 850, sea temperature of 15C, air temperature of 20C, and wave height of 2 meters?"

**🤖 AI Agent:**
> After 48 hours, the remaining volume is 385 cubic meters, with an emulsification percentage of 12% and a viscosity increase factor of 1.15.

---

**👤 You:**
> "Assess the risk for a spill with 200 cubic meters remaining, located 5 kilometers from the coast, which is currently emulsified."

**🤖 AI Agent:**
> The risk level is High, with the primary concern being the emulsification state which complicates cleanup efforts near the coastline.


## ❓ FAQ

**Q: How can I predict where the oil will move?**
You can use the `get_spill_trajectory` tool by providing the initial spill volume, coordinates, wind and current conditions, and the duration of the simulation.

**Q: Can I determine if the oil will hit the coast?**
Yes, the `predict_shoreline_impact` tool uses a previously calculated trajectory to estimate if and when the oil will contact a defined shoreline boundary.

**Q: How is the environmental risk calculated?**
The `get_spill_risk_assessment` tool evaluates risk based on the remaining oil volume, the distance to the nearest coast, and the current emulsification state of the oil.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tanker-spill-response-modeling](https://vinkius.com/en/ai-agent-connect/tanker-spill-response-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tanker Spill Response Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tanker-spill-response-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tanker Spill Response Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tanker-spill-response-modeling": {
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

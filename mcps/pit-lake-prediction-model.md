# Pit Lake Prediction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pit-lake-prediction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Predicts pit lake formation, water levels, and water quality evolution.

## Description
This MCP server provides specialized tools for mining engineers to model the lifecycle of pit lakes. It calculates the time required for a pit to fill using `calculate_filling_status`, projects future water levels with `predict_water_level_evolution`, and simulates chemical changes through `simulate_water_quality`. It also quantifies mineral dissolution using `evaluate_leaching_impact` to understand how wall rock chemistry affects water quality over time.


## Available Tools (4)
- **predict_water_level_evolution**: Projects the water level at specific future time intervals
- **simulate_water_quality**: Models the chemical changes in the lake over time due to mineral interactions
- **calculate_filling_status**: Determines how much time is required for the pit to fill and the current state of the water level
- **evaluate_leaching_impact**: Quantifies the specific contribution of wall rock dissolution to the total water chemistry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pit Lake Prediction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take for the pit to fill given the current geometry and rainfall?"

**🤖 AI Agent:**
> Based on the provided geometry and water balance, the pit is expected to reach its final water level in 12.5 years.

---

**👤 You:**
> "What will the water level be in 10 years?"

**🤖 AI Agent:**
> In 10 years, the projected water level is 45.2 meters.

---

**👤 You:**
> "How will the water quality change due to the reactive wall rock?"

**🤖 AI Agent:**
> The simulation shows that the pH level will decrease to 5.4 and metal concentrations will increase due to the leaching of reactive minerals.


## ❓ FAQ

**Q: How does the model account for evaporation?**
The model incorporates evaporation rates into the water balance calculations to determine the net accumulation of water in the pit.

**Q: Can I simulate the impact of specific rock types?**
Yes, by using `simulate_water_quality`, you can model how different mineral compositions in the wall rock influence pH and metal concentrations.

**Q: What data is required for filling status calculations?**
You need to provide pit geometry, annual rainfall, annual groundwater inflow, and annual evaporation rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pit-lake-prediction-model](https://vinkius.com/ai-agent-connect/pit-lake-prediction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pit Lake Prediction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pit-lake-prediction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pit Lake Prediction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pit-lake-prediction-model": {
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

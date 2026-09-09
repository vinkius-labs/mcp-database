# Groundwater Inflow Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/groundwater-inflow-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [hydrology](../categories/hydrology.md)

Predicts groundwater inflow, drawdown, and seepage patterns for excavations.

## Description
This MCP server provides analytical tools to model groundwater behavior around excavations. It allows users to calculate steady-state inflow using `get_steady_state_inflow`, model time-dependent progression with `get_transient_inflow_progression`, map water level reductions via `calculate_drawdown_profile`, and evaluate flow directionality through `analyze_seepage_patterns`.


## Available Tools (4)
- **analyze_seepage_patterns**: Determines the direction and intensity of water movement
- **calculate_drawdown_profile**: Maps the reduction in water level at various distances from the excavation
- **get_steady_state_inflow**: Calculates the steady-state groundwater inflow rate into an excavation
- **get_transient_inflow_progression**: Predicts the time-dependent progression of groundwater inflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groundwater Inflow Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the steady-state inflow for an aquifer with 1e-4 permeability, 10m thickness, 0.05 gradient, and 50m perimeter?"

**🤖 AI Agent:**
> The steady-state inflow rate is 2.5 m³/s with a total drawdown of 4.2m and a seepage velocity of 0.15 m/s.

---

**👤 You:**
> "Predict the inflow progression starting at 10 m³/s, heading to 50 m³/s, with storativity of 0.2 at times 1, 5, and 10 minutes."

**🤖 AI Agent:**
> At 1 minute, the inflow is 15.2 m³/s; at 5 minutes, it is 32.8 m³/s; and at 10 minutes, it reaches 41.5 m³/s.

---

**👤 You:**
> "Analyze the seepage patterns for an excavation 20m wide, 15m deep, with a 0.03 hydraulic gradient."

**🤖 AI Agent:**
> The water flow is convergent with an intensity index of 0.85 and a convergence factor of 1.2.


## ❓ FAQ

**Q: How do I calculate the equilibrium inflow rate?**
You can use the `get_steady_state_inflow` tool by providing the aquifer permeability, thickness, hydraulic gradient, and excavation perimeter.

**Q: Can I model how inflow changes over time?**
Yes, the `get_transient_inflow_progression` tool predicts how the inflow rate evolves from an initial state toward equilibrium.

**Q: How is drawdown measured?**
The `calculate_drawdown_profile` tool maps the reduction in water level at specific distances from the excavation edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/groundwater-inflow-predictor](https://vinkius.com/ai-agent-connect/groundwater-inflow-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groundwater Inflow Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groundwater-inflow-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groundwater Inflow Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groundwater-inflow-predictor": {
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

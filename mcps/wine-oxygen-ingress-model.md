# Wine Oxygen Ingress Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predictive modeling for oxygen ingress and wine aging trajectories.

## Description
This MCP server provides a predictive modeling engine to simulate oxygen transmission through different cork materials. It allows AI agents to estimate wine aging trajectories by calculating annual oxygen ingress using `calculate_annual_ingress`, predicting when oxygen levels reach critical thresholds with `predict_oxygen_saturation_timing`, and determining the chemical state of the wine via `predict_wine_evolution_state`. It also accounts for thermal fluctuations using `simulate_temperature_impact` to adjust ingress and consumption rates.


## Available Tools (4)
- **calculate_annual_ingress**: Calculate the total mass of oxygen entering the wine in a single year
- **predict_oxygen_saturation_timing**: Estimate when oxygen levels in the wine will reach a critical threshold
- **predict_wine_evolution_state**: Categorize the predicted chemical state of the wine
- **simulate_temperature_impact**: Adjust ingress and consumption parameters based on thermal fluctuations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Oxygen Ingress Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the annual oxygen ingress for a natural cork with an OTR of 0.5, stored horizontally at 15 degrees Celsius."

**🤖 AI Agent:**
> The annual oxygen ingress for the natural cork is 12.45 mg/L.

---

**👤 You:**
> "Predict the wine evolution state for a high sensitivity wine with 50 mg/L cumulative oxygen exposure."

**🤖 AI Agent:**
> The predicted evolution state is Oxidative.

---

**👤 You:**
> "When will the oxygen reach saturation if initial dissolved oxygen is 0.5 mg/L, annual ingress is 10 mg/L, and consumption is 2 mg/L?"

**🤖 AI Agent:**
> The oxygen saturation is predicted to occur in 0.6 months.


## ❓ FAQ

**Q: What cork types are supported?**
The model supports natural, technical, and agglomerate cork types.

**Q: How does storage position affect the results?**
Storage position (horizontal or vertical) changes the contact surface area between the wine and the cork, which is factored into the `calculate_annual_ingress` tool.

**Q: Can I model the impact of temperature changes?**
Yes, you can use `simulate_temperature_impact` to adjust ingress and consumption parameters based on thermal deviations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-model](https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Oxygen Ingress Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-oxygen-ingress-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Oxygen Ingress Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-oxygen-ingress-model": {
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

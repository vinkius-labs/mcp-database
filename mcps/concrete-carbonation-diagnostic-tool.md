# Concrete Carbonation Diagnostic Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-carbonation-diagnostic-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Predict carbonation depth, corrosion timing, and remaining service life for reinforced concrete structures.

## Description
This MCP server provides professional-grade diagnostic tools for predicting the degradation of reinforced concrete due to atmospheric CO2. By modeling the diffusion of carbon dioxide into the concrete matrix, the server allows AI agents to assess structural health. Use `calculate_current_depth` to find existing penetration, `predict_time_to_corrosion` to forecast when the carbonation front hits the steel, and `calculate_remaining_service_life` to determine safe operating years. You can also use `evaluate_exposure_risk` to classify environmental severity based on CO2 and humidity levels.


## Available Tools (4)
- **calculate_remaining_service_life**: Provides the remaining safe operating years for a structure given its current age and cover
- **evaluate_exposure_risk**: Classifies the environmental severity and the resulting impact on concrete durability
- **predict_time_to_corrosion**: Forecasts the specific year when the carbonation front will reach the steel reinforcement
- **calculate_current_depth**: Determines how deep carbonation has penetrated at a specific point in the structure's history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Carbonation Diagnostic Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current carbonation depth for a 30MPa concrete with 5% CO2 and 60% humidity after 10 years?"

**🤖 AI Agent:**
> The current carbonation depth is 4.25 mm.

---

**👤 You:**
> "How many years of service life remain for a structure with 40mm cover, 35MPa strength, 4% CO2, and 50% humidity, if it is already 5 years old?"

**🤖 AI Agent:**
> The remaining service life is 35 years, with a total life expectancy of 40 years.

---

**👤 You:**
> "Assess the exposure risk for an environment with 6% CO2 and 70% humidity."

**🤖 AI Agent:**
> The risk level is High, as high CO2 combined with moderate humidity accelerates carbonation significantly.


## ❓ FAQ

**Q: How does concrete strength affect carbonation?**
Higher concrete strength typically results in lower permeability, which slows the ingress of CO2 and extends the service life.

**Q: What is the significance of relative humidity in these calculations?**
Carbonation requires moisture for the chemical reaction. The tool uses humidity to determine the optimal rate of CO2 diffusion through the concrete pores.

**Q: Can I predict when my structure will need repair?**
Yes, by using `predict_time_to_corrosion`, you can forecast the specific year the carbonation front reaches the reinforcement, signaling the need for intervention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-carbonation-diagnostic-tool](https://vinkius.com/ai-agent-connect/concrete-carbonation-diagnostic-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Carbonation Diagnostic Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-carbonation-diagnostic-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Carbonation Diagnostic Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-carbonation-diagnostic-tool": {
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

# Wellbore Heat Transfer Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellbore-heat-transfer-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates temperature profiles and thermal energy exchange in producing or injecting wells.

## Description
This MCP server provides specialized thermal modeling for wellbore operations. It connects AI agents to advanced heat transfer calculations, allowing for the determination of temperature profiles at specific depths using `get_temperature_profile`. Users can measure total thermal energy exchange with `calculate_heat_exchange`, determine surface temperatures via `get_wellhead_temperature`, and predict time-dependent thermal changes using `simulate_transient_effect`. The engine accounts for geothermal gradients, fluid properties, and wellbore configurations to provide accurate thermal dynamics for geothermal and petroleum engineering workflows.


## Available Tools (4)
- **simulate_transient_effect**: Predicts how the temperature profile changes over a specific period of time
- **get_temperature_profile**: Determines the temperature of the fluid at a specific depth within the well
- **get_wellhead_temperature**: Calculates the temperature of the fluid at the surface (wellhead)
- **calculate_heat_exchange**: Measures the total thermal energy gained or lost by the fluid over the entire length of the well


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellbore Heat Transfer Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the temperature at 1500 meters depth for a well with a 100m total depth and a geothermal gradient of 0.03 deg/m?"

**🤖 AI Agent:**
> The temperature at 1500 meters is 55.2°C.

---

**👤 You:**
> "Calculate the total heat loss for this well."

**🤖 AI Agent:**
> The total heat loss for the well is 450.5 kJ.

---

**👤 You:**
> "What will the wellhead temperature be if the bottom-hole temperature is 80°C?"

**🤖 AI Agent:**
> The estimated wellhead temperature is 62.4°C.


## ❓ FAQ

**Q: How accurate are the temperature calculations?**
The engine uses Ramey's model and numerical heat transfer methods to provide high-fidelity temperature profiles based on the provided fluid properties and wellbore geometry.

**Q: Can I simulate how temperature changes over time?**
Yes, you can use the `simulate_transient_effect` tool to predict how the temperature profile evolves over a specific duration.

**Q: What inputs are required for heat exchange calculations?**
To use `calculate_heat_exchange`, you need to provide the well configuration, fluid properties, geothermal gradient, and the volumetric flow rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellbore-heat-transfer-engine](https://vinkius.com/en/ai-agent-connect/wellbore-heat-transfer-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellbore Heat Transfer Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellbore-heat-transfer-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellbore Heat Transfer Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellbore-heat-transfer-engine": {
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

# Hydraulic Conductivity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hydraulic-conductivity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates saturated and unsaturated hydraulic conductivity using physical soil properties.

## Description
This MCP server provides specialized tools for geotechnical and hydrological analysis. It allows AI agents to calculate saturated hydraulic conductivity ($K_{sat}$) using the Kozeny-Carman relationship and determine unsaturated conductivity via the van Genuchten-Mualem model. Users can also analyze pore size distribution and calculate temperature-based viscosity adjustments to ensure accurate flow modeling in various environmental conditions.


## Available Tools (4)
- **get_saturated_conductivity**: Calculates the maximum water flow capacity when the medium is fully saturated
- **get_unsaturated_conductivity**: Determines the water flow rate when the medium is partially saturated
- **get_pore_size_distribution**: Analyzes the internal structure of the medium to understand how pore sizes are distributed
- **get_viscosity_adjustment**: Calculates the specific multiplier needed to adjust conductivity based on temperature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydraulic Conductivity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the saturated hydraulic conductivity for a soil with particle size 0.002, porosity 0.4, bulk density 1.5, and temperature 20."

**🤖 AI Agent:**
> The calculated saturated hydraulic conductivity (Ksat) is 1.25e-5 m/s with a temperature correction factor of 1.0.

---

**👤 You:**
> "What is the viscosity adjustment factor for water at 40 degrees Celsius compared to a reference of 20 degrees?"

**🤖 AI Agent:**
> The adjustment factor for 40°C is 1.54.

---

**👤 You:**
> "Analyze the pore size distribution for a sample with porosity 0.35 and particle sizes [0.001, 0.002, 0.005, 0.01]."

**🤖 AI Agent:**
> The distribution index is 0.12 and the dominant pore size is 0.005.


## ❓ FAQ

**Q: How do I calculate saturated conductivity?**
You can use the `get_saturated_conductivity` tool by providing the particle size, porosity, bulk density, and temperature.

**Q: Can this tool account for temperature changes?**
Yes, the `get_viscosity_adjustment` tool calculates the multiplier needed to adjust conductivity based on water viscosity changes at different temperatures.

**Q: How is unsaturated flow modeled?**
Unsaturated flow is modeled using the `get_unsaturated_conductivity` tool, which implements the van Genuchten-Mualem framework.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hydraulic-conductivity-calculator](https://vinkius.com/ai-agent-connect/hydraulic-conductivity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydraulic Conductivity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydraulic-conductivity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydraulic Conductivity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydraulic-conductivity-calculator": {
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

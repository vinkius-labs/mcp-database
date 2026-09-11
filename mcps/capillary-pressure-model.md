# Capillary Pressure Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/capillary-pressure-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates capillary pressure curves, threshold pressure, and transition zone thickness.

## Description
This MCP server provides specialized tools for reservoir engineering and soil science. It allows AI agents to calculate capillary pressure curves using the Brooks-Corey model, determine the threshold pressure for fluid entry, and estimate the thickness of fluid transition zones. Users can also normalize data using the `scale_via_leverett_j` tool to compare different porous media. The server handles both drainage and imbibition processes to account for hysteresis.


## Available Tools (4)
- **estimate_transition_zone_thickness**: estimate_transition_zone_thickness
- **calculate_capillary_pressure_curve**: Generates capillary pressure curves
- **get_threshold_pressure**: get_threshold_pressure
- **scale_via_leverett_j**: scale_via_leverett_j


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capillary Pressure Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the threshold pressure for a medium with this pore size distribution: [{"diameter": 0.005, "volumeFraction": 0.2}, {"diameter": 0.01, "volumeFraction": 0.8}] and an interfacial tension of 0.03?"

**🤖 AI Agent:**
> The threshold pressure for the provided pore size distribution and interfacial tension is 150.5 kPa.

---

**👤 You:**
> "Calculate the transition zone thickness given a pressure curve with saturations [0.2, 0.5, 0.8] and pressures [10, 50, 100], permeability of 150 mD, porosity of 0.2, gravity of 9.8, and a density difference of 500 kg/m³."

**🤖 AI Agent:**
> The estimated transition zone thickness is 1.24 meters.

---

**👤 You:**
> "Generate a capillary pressure curve for a water-wet medium in drainage mode."

**🤖 AI Agent:**
> The generated drainage curve shows a gradual pressure increase starting from a threshold of 25.0 kPa.


## ❓ FAQ

**Q: How do I calculate the entry pressure for a new medium?**
You can use the `get_threshold_pressure` tool by providing the pore size distribution, interfacial tension, and wettability.

**Q: Can I model both drainage and imbibition?**
Yes, the `calculate_capillary_pressure_curve` tool supports both 'drainage' and 'imbibition' modes to account for hysteresis.

**Q: How can I compare different reservoir units?**
Use the `scale_via_leverett_j` tool to normalize your capillary pressure curves into a dimensionless form.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/capillary-pressure-model](https://vinkius.com/en/ai-agent-connect/capillary-pressure-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Capillary Pressure Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `capillary-pressure-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Capillary Pressure Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capillary-pressure-model": {
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

# Wave Diffraction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-diffraction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [physics-simulation](../categories/physics-simulation.md)

Models wave diffraction around maritime obstacles like breakwaters and headlands.

## Description
This MCP server provides specialized tools for maritime engineering and oceanography. It models how wave energy redistributes when encountering physical obstacles. Using diffraction theory, it allows AI agents to calculate the `get_diffraction_coefficient` for specific points, determine the `calculate_shadow_zone_height` in protected areas, generate an `get_energy_distribution_map` for spatial analysis, and use `analyze_obstacle_type_effect` to compare how different geometries like breakwaters or headlands influence wave patterns.


## Available Tools (4)
- **calculate_shadow_zone_height**: Calculate wave height in shadow zone
- **analyze_obstacle_type_effect**: Analyze obstacle type effect
- **get_diffraction_coefficient**: Calculate diffraction coefficient
- **get_energy_distribution_map**: Get energy distribution map


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Diffraction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much has the wave height decreased at a point 50m behind a 100m breakwater with a 10m wavelength at a 30 degree angle?"

**🤖 AI Agent:**
> The diffraction coefficient at that location is 0.45.

---

**👤 You:**
> "What is the wave height in the shadow zone if the incident wave is 3m, wavelength is 15m, obstacle is 200m, distance is 40m, and angle is 10 degrees?"

**🤖 AI Agent:**
> The resulting wave height at that target point is 0.85m.

---

**👤 You:**
> "Compare the impact of a breakwater versus a headland for a 12m wavelength at a 45 degree angle."

**🤖 AI Agent:**
> The breakwater produces a more predictable linear shadow zone, while the headland creates a more complex, curved energy pattern with an impact factor of 1.24.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the diffraction coefficient, the specific wave height in shadow zones, the energy distribution across a coordinate grid, and the impact of different obstacle types.

**Q: Does it support both breakwaters and headlands?**
Yes, the `analyze_obstacle_type_effect` tool specifically allows you to compare the diffraction patterns of breakwaters versus natural headlands.

**Q: How is the energy distribution map generated?**
The `get_energy_distribution_map` tool generates a grid of coordinates and energy density values based on the provided wavelength, obstacle length, and search radius.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-diffraction-model](https://vinkius.com/en/ai-agent-connect/wave-diffraction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Diffraction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-diffraction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Diffraction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-diffraction-model": {
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

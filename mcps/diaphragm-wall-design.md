# Diaphragm Wall Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/diaphragm-wall-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Simulate staged excavation and calculate structural demands for diaphragm walls.

## Description
This MCP server provides specialized engineering tools for designing diaphragm walls in deep excavations. It simulates the staged excavation process to calculate critical structural responses, including wall moment and shear diagrams. Engineers can use `analyze_wall_stability` to determine maximum forces, `calculate_strut_loads` to find axial compressive loads on support systems, and `determine_embedment_requirement` to ensure stability against sliding or kicking out. It also allows querying specific soil properties at any depth using `get_soil_properties_at_depth`.


## Available Tools (4)
- **calculate_strut_loads**: Determines the compressive forces acting on each installed strut
- **determine_embedment_requirement**: Calculates the minimum depth the wall must be embedded below the excavation base to ensure stability
- **get_soil_properties_at_depth**: Retrieves the specific physical properties of the soil at a requested vertical coordinate
- **analyze_wall_stability**: Calculates the primary structural responses of the wall throughout the excavation process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diaphragm Wall Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stability of a 15m excavation with a 0.8m thick wall and a water table at 3m."

**🤖 AI Agent:**
> The analysis shows a maximum bending moment of 450 kNm/m and a maximum shear force of 120 kN/m for the specified excavation depth and soil profile.

---

**👤 You:**
> "What are the forces on struts installed at 5m and 10m for this excavation?"

**🤖 AI Agent:**
> The strut at 5m is experiencing a compressive force of 250 kN, and the strut at 10m is experiencing 310 kN.

---

**👤 You:**
> "How deep must the wall be embedded for a 20m excavation?"

**🤖 AI Agent:**
> The minimum required embedment depth to ensure stability is 6.5 meters.


## ❓ FAQ

**Q: How does the tool handle water pressure?**
The tool accounts for hydrostatic pressure by using the provided groundwater level to calculate the additional lateral pressure acting on the wall and the soil.

**Q: Can I calculate the forces on my support struts?**
Yes, you can use the `calculate_strut_loads` tool to determine the axial compressive forces acting on each strut at specific depths.

**Q: What information is needed for stability analysis?**
To perform a stability analysis, you need to provide the excavation depth, the soil profile, the groundwater level, and the wall thickness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/diaphragm-wall-design](https://vinkius.com/ai-agent-connect/diaphragm-wall-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diaphragm Wall Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diaphragm-wall-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diaphragm Wall Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diaphragm-wall-design": {
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

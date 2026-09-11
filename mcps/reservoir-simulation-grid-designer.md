# Reservoir Simulation Grid Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reservoir-simulation-grid-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimizes spatial discretization for reservoir engineering simulations.

## Description
This MCP server provides specialized tools for reservoir engineering to design efficient simulation grids. It allows users to `calculate_optimal_cell_size` to balance physical accuracy with computational limits, `assess_well_influence_resolution` to ensure pressure gradients near wells are captured, `estimate_upscaling_impact` to predict information loss, and `optimize_grid_for_constraints` to fit designs within hardware limits.


## Available Tools (4)
- **optimize_grid_for_constraints**: Adjusts the grid design to fit within specific hardware or time constraints
- **assess_well_influence_resolution**: Evaluates if the proposed grid is fine enough to capture the pressure and saturation gradients around wells
- **calculate_optimal_cell_size**: Determines the ideal spatial resolution required to balance physical accuracy with computational limits
- **estimate_upscaling_impact**: Predicts the level of information loss when moving from a fine-scale geological model to the simulation grid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Simulation Grid Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best cell size for a reservoir 1000m long, 500m wide, with a heterogeneity scale of 50m and a 10 minute limit?"

**🤖 AI Agent:**
> The optimal cell size for these parameters is 25m x 25m, resulting in a total of 800 cells.

---

**👤 You:**
> "Will my current grid capture the pressure changes near my wells?"

**🤖 AI Agent:**
> The resolution is adequate for the current well spacing and cell size.

---

**👤 You:**
> "How much information will I lose if I upscale from 1m to 10m resolution for permeability?"

**🤖 AI Agent:**
> The predicted information loss index is 0.15, which indicates high accuracy confidence for permeability.


## ❓ FAQ

**Q: How do I ensure my grid captures well-bore effects?**
You can use the `assess_well_influence_resolution` tool to evaluate if your cell size is adequate relative to your well spacing.

**Q: Can I adjust my grid to fit specific hardware limits?**
Yes, the `optimize_grid_for_constraints` tool helps adjust the cell count and dimensions to stay within your target computational capacity.

**Q: How is the optimal cell size determined?**
The `calculate_optimal_cell_size` tool uses reservoir dimensions and the heterogeneity scale to find the ideal resolution for your simulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reservoir-simulation-grid-designer](https://vinkius.com/ai-agent-connect/reservoir-simulation-grid-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Simulation Grid Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-simulation-grid-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Simulation Grid Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-simulation-grid-designer": {
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

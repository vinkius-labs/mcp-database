# Reservoir Simulation Upscaling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-simulation-upscaling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Upscale fine-scale geological models to simulation grids.

## Description
This MCP server provides tools to transform high-resolution geological data into coarser grids for reservoir simulation. It enables the calculation of effective properties like porosity, Net-to-Gross (NTG), and permeability. Users can apply analytical methods via `upscale_permeability_simple` or perform advanced simulations using `upscale_permeability_flow_based` to capture complex heterogeneity and anisotropy.


## Available Tools (4)
- **upscale_ntg**: Determines the Net-to-Gross ratio for a coarse-scale cell
- **upscale_permeability_flow_based**: Estimates effective permeability by simulating local flow
- **upscale_permeability_simple**: Calculates effective permeability using analytical averaging methods
- **upscale_porosity**: Calculates the coarse-scale porosity for a defined volume of fine-scale cells


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Simulation Upscaling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the coarse-scale porosity for these fine cells: porosities [0.2, 0.25, 0.18] and volumes [10, 15, 5]."

**🤖 AI Agent:**
> The coarse-scale porosity is 0.216.

---

**👤 You:**
> "What is the Net-to-Gross ratio if the fine cell volumes are [10, 10, 10] and the first two cells are reservoir rock?"

**🤖 AI Agent:**
> The Net-to-Gross ratio is 0.667.

---

**👤 You:**
> "Use arithmetic averaging for permeabilities [10, 20, 30]."

**🤖 AI Agent:**
> The effective permeability is 20.


## ❓ FAQ

**Q: What is the difference between the permeability methods?**
The `upscale_permeability_simple` tool offers arithmetic, harmonic, and power-average methods for analytical estimation, while `upscale_permeability_flow_based` uses local numerical simulation to better account for spatial heterogeneity.

**Q: How is porosity calculated?**
Porosity is calculated as a volume-weighted average of the fine-scale cells using the `upscale_porosity` tool.

**Q: Can I calculate Net-to-Gross (NTG)?**
Yes, the `upscale_ntg` tool determines the ratio of productive reservoir rock volume to the total volume of the coarse cell.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-simulation-upscaling](https://vinkius.com/en/ai-agent-connect/reservoir-simulation-upscaling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Simulation Upscaling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-simulation-upscaling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Simulation Upscaling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-simulation-upscaling": {
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

# Surface Area Measurement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/surface-area-measurement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate specific surface area and monolayer capacity using BET isotherm analysis.

## Description
This MCP server provides specialized tools for analyzing adsorption isotherms using Brunauer-Emmett-Teller (BET) theory. It allows AI agents to determine the specific surface area of materials by processing gas adsorption data. Key capabilities include using `get_bet_constants` to retrieve physical properties for gases like nitrogen, `calculate_linear_bet_region` to identify valid pressure ranges, `compute_bet_parameters` to find the C constant and monolayer capacity, and `calculate_specific_surface_area` to produce the final surface area measurement in m²/g.


## Available Tools (4)
- **get_bet_constants**: g., "nitrogen", to get its molecular cross-sectional area and saturation vapor pressure.

Retrieve physical constants for specific gases used in adsorption experiments
- **calculate_linear_bet_region**: Identify the optimal range of relative pressure (P/P0) for the BET equation
- **calculate_specific_surface_area**: Convert monolayer capacity into specific surface area
- **compute_bet_parameters**: Calculate fundamental BET parameters (C constant and Monolayer Capacity)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surface Area Measurement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the physical constants for nitrogen?"

**🤖 AI Agent:**
> For nitrogen, the molecular cross-sectional area is 0.162 nm² and the saturation vapor pressure is 101325 Pa.

---

**👤 You:**
> "Calculate the specific surface area for a 0.5g sample with a monolayer capacity of 0.002 moles and a molecular area of 0.162e-18 m²."

**🤖 AI Agent:**
> The calculated specific surface area is 243.6 m²/g.

---

**👤 You:**
> "Find the linear BET region for these relative pressures: [0.05, 0.1, 0.15, 0.2, 0.25] and adsorption amounts: [0.01, 0.02, 0.03, 0.04, 0.05]."

**🤖 AI Agent:**
> The valid linear range is between 0.05 and 0.25 with an R-squared value of 0.999.


## ❓ FAQ

**Q: What is BET theory?**
BET (Brunauer-Emmett-Teller) theory is a physical model used to determine the specific surface area of particulate solids by measuring how gas molecules adsorb onto the surface at various pressures.

**Q: Which gases are supported?**
The server supports standard gases used in adsorption experiments, such as nitrogen, argon, and carbon dioxide, via the `get_bet_constants` tool.

**Q: How do I calculate the final surface area?**
You can use the `calculate_specific_surface_area` tool by providing the monolayer capacity, the molecular cross-sectional area, and the sample mass.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/surface-area-measurement](https://vinkius.com/ai-agent-connect/surface-area-measurement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surface Area Measurement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surface-area-measurement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surface Area Measurement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surface-area-measurement": {
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

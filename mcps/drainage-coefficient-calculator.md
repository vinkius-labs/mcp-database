# Drainage Coefficient Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/drainage-coefficient-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Design optimal tile drainage systems by calculating drainage coefficients, spacing, and depth.

## Description
This MCP server provides technical tools for designing efficient tile drainage systems. It helps engineers and agronomists balance water removal needs with crop requirements. Use `design_system_summary` to generate a complete design package including drainage coefficient, spacing, and depth. You can also use `get_drainage_coefficient` to determine specific removal rates or `calculate_drain_spacing` and `calculate_drain_depth` for individual component design. The tool accounts for soil permeability, rainfall intensity, crop waterlogging tolerance, and land slope, including specialized support for subirrigation mode.


## Available Tools (4)
- **calculate_drain_depth**: Determines the appropriate vertical placement for the drainage pipes
- **calculate_drain_spacing**: Determines the optimal distance between lateral drain pipes
- **design_system_summary**: Provides a complete design package (coefficient, spacing, and depth) for a specific field setup
- **get_drainage_coefficient**: Determines the required rate of water removal for a specific scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drainage Coefficient Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Provide a complete drainage system design for a field with 5cm rainfall, 0.5 soil permeability, 0.8 crop tolerance, and 1% slope."

**🤖 AI Agent:**
> The recommended design is a drainage coefficient of 1.2 cm/day, drain spacing of 15.5 meters, and a drain depth of 110 cm.

---

**👤 You:**
> "What is the required drainage coefficient for a 10cm storm with 0.2 soil permeability and 0.5 crop tolerance?"

**🤖 AI Agent:**
> The required drainage coefficient is 4.5 cm/day.

---

**👤 You:**
> "Calculate the drain spacing for a coefficient of 2.0, permeability of 0.4, depth of 100, and slope of 2."

**🤖 AI Agent:**
> The optimal drain spacing is 22.4 meters.


## ❓ FAQ

**Q: How do I design a full drainage system?**
Use the `design_system_summary` tool. It will calculate the drainage coefficient, spacing, and depth in one go based on your field parameters.

**Q: Can this tool handle subirrigation?**
Yes, by setting the `isSubirrigationMode` parameter to true, the tools will adjust calculations to support raising the water table for crop needs.

**Q: What inputs are required for spacing calculations?**
To use `calculate_drain_spacing`, you need the drainage coefficient, soil permeability, drain depth, and the ground slope.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/drainage-coefficient-calculator](https://vinkius.com/ai-agent-connect/drainage-coefficient-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drainage Coefficient Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drainage-coefficient-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drainage Coefficient Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drainage-coefficient-calculator": {
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

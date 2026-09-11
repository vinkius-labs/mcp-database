# Column Flotation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/column-flotation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design mineral processing column flotation circuits with precise geometry and hydraulic calculations.

## Description
This MCP server provides specialized engineering tools for designing mineral processing column flotation circuits. It allows AI agents to calculate essential physical dimensions such as column height and diameter using `calculate_column_geometry`. Users can specify air distribution systems via `design_sparger_configuration`, evaluate the impact of wash water on concentrate purity with `evaluate_wash_water_impact`, and determine optimal operating setpoints through `optimize_circuit_parameters`. It is built for metallurgical engineers to bridge the gap between feed characteristics and optimized flotation performance.


## Available Tools (4)
- **design_sparger_configuration**: Specifies the air distribution system needed to generate the appropriate bubble size for the given feed
- **evaluate_wash_water_impact**: Calculates how much wash water is needed and how it will affect the concentrate purity and bias
- **optimize_circuit_parameters**: Provides a final set of optimized operating setpoints based on the established geometry and water constraints
- **calculate_column_geometry**: Determines the physical dimensions of the flotation column required to meet specific recovery goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Column Flotation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the column dimensions for a feed with 15% grade, a 90% recovery target, and a mass flow rate of 50 t/h."

**🤖 AI Agent:**
> The required column height is 8.5 meters, the diameter is 1.2 meters, and the total volume is 9.94 cubic meters.

---

**👤 You:**
> "What is the impact of using 5 m3/h of wash water on a 1.2m diameter column for a 95% target grade?"

**🤖 AI Agent:**
> Using 5 m3/h of wash water will result in an expected grade improvement of 4.2% and a resulting bias of 1.15.

---

**👤 You:**
> "Design a sparger for a 1.2m diameter column with a fine particle size distribution."

**🤖 AI Agent:**
> The recommended sparger type is a porous plate with an orifice diameter of 2.5mm and an air flow capacity of 15 m3/h.


## ❓ FAQ

**Q: What parameters are needed for column geometry?**
To use `calculate_column_geometry`, you need the feed grade, target recovery, and mass flow rate.

**Q: How does wash water affect the design?**
The `evaluate_wash_water_impact` tool calculates how wash water improves concentrate grade by removing gangue while maintaining the required bias.

**Q: Can I optimize the entire circuit at once?**
Yes, once you have the column dimensions, you can use `optimize_circuit_parameters` to find the best air flow, wash water rate, and superficial velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/column-flotation-design](https://vinkius.com/en/ai-agent-connect/column-flotation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Column Flotation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `column-flotation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Column Flotation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "column-flotation-design": {
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

# Grassed Waterway Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/grassed-waterway-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design stable grassed waterways using hydraulic modeling and vegetation retardance.

## Description
This MCP server provides specialized engineering tools for designing grassed waterways that manage concentrated water flow. By applying Manning's equation and accounting for vegetation retardance, the server calculates critical dimensions like width and depth. It helps engineers assess erosion risks during the vegetation establishment period and compare different channel geometries, such as parabolic and trapezoidal shapes, to ensure hydraulic stability and long-term functionality.


## Available Tools (4)
- **estimate_maintenance_schedule**: Provides a long-term plan for keeping the waterway functional and stable
- **calculate_waterway_dimensions**: Determines the physical size and shape of the waterway needed to accommodate peak runoff
- **compare_shapes**: Compares the hydraulic efficiency and stability of different channel geometries
- **evaluate_establishment_risk**: Assesses the risk of erosion during the period before vegetation is fully grown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grassed Waterway Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a waterway with a 50 acre drainage area, 10 cfs runoff, 2% slope, Silty soil, and Fast-Growth vegetation using a parabolic shape."

**🤖 AI Agent:**
> The required waterway dimensions are a width of 12.5 feet and a depth of 2.1 feet, with a calculated velocity of 3.4 feet per second.

---

**👤 You:**
> "What is the maintenance plan for a 15-foot wide waterway with Low-Maintenance vegetation on Loam soil?"

**🤖 AI Agent:**
> The maintenance frequency is 1 time per year, with primary tasks including sediment removal and checking for erosion at the channel edges.

---

**👤 You:**
> "Compare parabolic and trapezoidal shapes for a site with a 100 acre drainage area and 3% slope."

**🤖 AI Agent:**
> The parabolic shape is recommended as it provides higher hydraulic efficiency and better stability for this specific slope and runoff rate.


## ❓ FAQ

**Q: How do I determine the size of my waterway?**
You can use the `calculate_waterway_dimensions` tool. Provide the drainage area, peak runoff rate, slope, soil type, vegetation type, and preferred shape to get the required width and depth.

**Q: Can I compare different channel shapes?**
Yes, the `compare_shapes` tool allows you to evaluate the hydraulic efficiency and stability of parabolic versus trapezoidal geometries for your specific site conditions.

**Q: How is erosion risk managed during plant growth?**
The `evaluate_establishment_risk` tool assesses the risk level and provides recommended protective measures for the period before vegetation is fully established.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/grassed-waterway-designer](https://vinkius.com/ai-agent-connect/grassed-waterway-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grassed Waterway Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grassed-waterway-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grassed Waterway Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grassed-waterway-designer": {
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

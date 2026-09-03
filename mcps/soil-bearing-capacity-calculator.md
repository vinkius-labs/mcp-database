# Soil Bearing Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soil-bearing-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate ultimate and allowable soil bearing capacity using Terzaghi's principles.

## Description
This MCP server provides essential geotechnical engineering tools to determine soil bearing capacity. It implements Terzaghi's bearing capacity theory, accounting for foundation geometry, soil properties, and groundwater influence. Engineers can use `get_capacity_summary` to generate complete reports or use specific tools like `calculate_ultimate_capacity` and `calculate_allowable_capacity` for targeted calculations. The toolset handles shape and depth factors, as well as buoyancy effects from groundwater, to provide accurate ultimate and safe working pressures.


## Available Tools (4)
- **calculate_allowable_capacity**: Determines the safe working pressure for foundation design
- **calculate_safety_factor**: Evaluates the current safety margin of a proposed loading scenario
- **calculate_ultimate_capacity**: Calculates the theoretical maximum soil pressure before shear failure occurs
- **get_capacity_summary**: Provides a complete engineering report for a specific foundation setup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil Bearing Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ultimate bearing capacity for a foundation 2m wide and 1.5m deep, with soil cohesion of 20 kPa, friction angle of 30 degrees, and unit weight of 18 kN/m³."

**🤖 AI Agent:**
> The calculated ultimate bearing capacity is 450.5 kPa.

---

**👤 You:**
> "What is the allowable bearing capacity if the ultimate capacity is 500 kPa and I need a safety factor of 3.0?"

**🤖 AI Agent:**
> The allowable bearing capacity is 166.67 kPa.

---

**👤 You:**
> "Check the safety factor for an applied pressure of 120 kPa when the ultimate capacity is 400 kPa."

**🤖 AI Agent:**
> The current safety factor is 3.33.


## ❓ FAQ

**Q: What theory does this tool use?**
The tool implements Terzaghi's bearing capacity theory, which is a fundamental method in geotechnical engineering for calculating soil strength.

**Q: How does groundwater affect the results?**
The presence of groundwater reduces the effective unit weight of the soil, which decreases the bearing capacity. The tool accounts for this buoyancy effect when `groundwaterDepth` is provided.

**Q: Can I get a full report for my foundation design?**
Yes, you can use the `get_capacity_summary` tool to receive a complete engineering report including ultimate capacity, allowable capacity, and the current safety factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soil-bearing-capacity-calculator](https://vinkius.com/ai-agent-connect/soil-bearing-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil Bearing Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-bearing-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil Bearing Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-bearing-capacity-calculator": {
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

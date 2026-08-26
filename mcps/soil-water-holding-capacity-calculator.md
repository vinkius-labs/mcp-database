# Soil Water Holding Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soil-water-holding-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate soil water retention, field capacity, and available water storage.

## Description
This MCP server provides precise soil moisture analysis tools. Use `get_soil_profile_summary` to obtain a complete diagnostic of soil water characteristics, including Field Capacity (FC), Permanent Wilting Point (PWP), and Available Water Capacity (AWC). You can also use `get_soil_water_retention` to determine volumetric water content based on sand, silt, and clay percentages, or `calculate_root_zone_storage` to find the total depth of water available in a specific soil layer in millimeters.


## Available Tools (4)
- **calculate_root_zone_storage**: Calculate the total depth of water available in a specific soil layer
- **get_soil_water_retention**: Determine volumetric water content at specific tension levels based on soil texture
- **calculate_available_water_capacity**: Calculate the amount of water available for plant uptake
- **get_soil_profile_summary**: Provide a complete diagnostic of the soil's water characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil Water Holding Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a full soil profile for a soil with 40% sand, 40% silt, 20% clay, 3% organic matter, a 500mm rooting depth, and 1.3 bulk density."

**🤖 AI Agent:**
> The soil profile shows a Field Capacity of 0.32, a Permanent Wilting Point of 0.12, an Available Water Capacity of 0.20, and a total water storage of 100 mm in the root zone.

---

**👤 You:**
> "What is the available water capacity for a soil with field capacity of 0.35 and wilting point of 0.15?"

**🤖 AI Agent:**
> The available water capacity is 0.20.

---

**👤 You:**
> "Calculate the water retention for 20% sand, 30% silt, and 50% clay with 2% organic matter."

**🤖 AI Agent:**
> The soil has a Field Capacity of 0.38 and a Permanent Wilting Point of 0.18.


## ❓ FAQ

**Q: What is Field Capacity?**
Field Capacity is the amount of soil moisture held in the soil after excess water has drained away due to gravity.

**Q: How does organic matter affect the results?**
Organic matter increases the soil's ability to hold water by improving structure and increasing surface area for moisture attachment.

**Q: Can I calculate total water storage in a specific depth?**
Yes, you can use the `calculate_root_zone_storage` tool to find the total depth of water available in millimeters for a given rooting depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soil-water-holding-capacity-calculator](https://vinkius.com/ai-agent-connect/soil-water-holding-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil Water Holding Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-water-holding-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil Water Holding Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-water-holding-capacity-calculator": {
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

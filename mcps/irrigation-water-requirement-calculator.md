# Irrigation Water Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/irrigation-water-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate crop evapotranspiration, water deficit, and required irrigation depths.

## Description
This MCP server provides specialized tools for precision agriculture. Use `calculate_phase_demand` to determine water demand and moisture deficit for specific growth stages of crops like Soybeans, Maize, Sugarcane, Coffee, or Cotton. With `calculate_irrigation_event_depth`, you can calculate the exact irrigation depth and volume needed based on accumulated deficits and application efficiency. Additionally, `get_crop_irrigation_profile` allows you to retrieve a complete seasonal water requirement overview for any supported crop.


## Available Tools (3)
- **get_crop_irrigation_profile**: Retrieve the seasonal water requirement profile for a crop
- **calculate_irrigation_event_depth**: Calculate required irrigation depth and volume
- **calculate_phase_demand**: Calculate water demand and deficit for a specific crop phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Irrigation Water Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the water demand for Soybeans in the Initial phase if I have 10 hectares and 5mm of rain?"

**🤖 AI Agent:**
> The water demand for the Initial phase of Soybeans is 12 mm, which corresponds to 120 m³/ha. The water deficit for this period is 7 mm.

---

**👤 You:**
> "I have a deficit of 15mm. How much irrigation depth do I need with 80% efficiency?"

**🤖 AI Agent:**
> To compensate for a 15 mm deficit with 80% efficiency, you need an irrigation depth of 18.75 mm, which is 187.5 m³/ha.

---

**👤 You:**
> "Show me the growth stages for Maize."

**🤖 AI Agent:**
> The Maize profile includes the following stages: Seedling, Development, Tasseling, and Grain-fill.


## ❓ FAQ

**Q: How do I calculate the water deficit for a specific crop stage?**
Use the `calculate_phase_demand` tool. You will need to provide the crop type, the phenological phase, the area in hectares, and the effective precipitation recorded during that period.

**Q: Can I calculate the volume of water needed for irrigation?**
Yes, by using the `calculate_irrigation_event_depth` tool. It calculates both the required depth in mm and the volumetric requirement in m³/ha based on your accumulated deficit.

**Q: Which crops are supported by this tool?**
The tool currently supports Soybeans, Maize, Sugarcane, Coffee, and Cotton.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/irrigation-water-requirement-calculator](https://vinkius.com/mcp/irrigation-water-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Irrigation Water Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `irrigation-water-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Irrigation Water Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "irrigation-water-requirement-calculator": {
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

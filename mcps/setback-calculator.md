# Setback Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/setback-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Determine maximum buildable area and optimal land utilization by applying local zoning setback rules.

## Description
**Need to know how much you can actually build on your lot?** Zoning laws dictate strict minimum setbacks (distances from property lines) that cannot be ignored. Ignoring these rules means building illegally and facing costly revisions.


## Available Tools
- **calculate_building_footprint**: Calculate the total buildable area and perimeter from usable envelope dimensions
- **calculate_land_utilization_metrics**: Percentage is capped at 100% if footprint exceeds total area.

Calculate how efficiently the plot is used by comparing built footprint area against total land area
- **calculate_usable_dimensions**: Returns the maximum allowable building envelope dimensions in meters.

Calculate the actual buildable dimensions after applying mandatory setback requirements to lot measurements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Setback Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a lot that is 40m long and 25m wide. My local code requires a 5m front setback, 3m rear setback, and 4m side setbacks on both sides. What are my buildable dimensions?"

**🤖 AI Agent:**
> To find this, I will execute the `calculate_usable_dimensions` tool with lotLengthMeters=40, lotWidthMeters=25, frontSetbackMeters=5, rearSetbackMeters=3, sideA_setbackMeters=4, and sideB_setbackMeters=4. The result will give me the maximum usable length and width.

---

**👤 You:**
> "Using my restricted dimensions of 32m by 17m, what is the total buildable area and perimeter?"

**🤖 AI Agent:**
> I will run `calculate_building_footprint` with usableLengthMeters=32 and usableWidthMeters=17. This provides the total footprint area in square meters, which is essential for zoning submissions.

---

**👤 You:**
> "If my lot's total area is 800 sq.m., and the building footprint is 512 sq.m., what percentage of land can I actually use?"

**🤖 AI Agent:**
> I will call `calculate_land_utilization_metrics` using totalLandAreaSqMeters=800 and buildingFootprintAreaSqMeters=512. This calculation gives the utilization percentage, confirming compliance.


## ❓ FAQ

**Q: What is the first step in calculating buildable dimensions?**
You must first use the `calculate_usable_dimensions` tool. This function takes your total lot size and mandatory setbacks (front, rear, side A, side B) to determine the absolute maximum buildable length and width.

**Q: How do I find the total area of my potential building?**
Once you have the usable dimensions, pass them to the `calculate_building_footprint` tool. This calculates the maximum rectangular area (the footprint) and its perimeter based on those restricted measurements.

**Q: Does this calculator tell me if my lot size is efficient?**
Yes. By using the `calculate_land_utilization_metrics` tool, you compare your calculated building footprint area against the total land area. This gives you a utilization percentage (0-100%), helping you assess zoning compliance risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/setback-calculator](https://vinkius.com/mcp/setback-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Setback Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `setback-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Setback Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "setback-calculator": {
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

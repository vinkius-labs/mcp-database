# Wine Cellar Capacity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-cellar-capacity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Plan winery cellar capacity, barrel inventory, and seasonal space utilization.

## Description
This MCP server provides essential tools for winery capacity planning. It helps winemakers manage the complex relationship between liquid volume and physical storage. Use `get_barrel_inventory_requirements` to determine the number of physical barrels needed based on aging regimes and turnover rates. Calculate necessary fermentation volumes with `get_tank_capacity_needs`. Visualize seasonal space usage through `get_seasonal_space_utilization` to prepare for peak production periods, and optimize barrel maintenance with `optimize_barrel_rotation` to ensure maximum availability.


## Available Tools (4)
- **get_seasonal_space_utilization**: Visualizes how cellar capacity changes throughout the year
- **get_barrel_inventory_requirements**: Determines how many physical barrels are needed to support the planned aging regimes
- **get_tank_capacity_needs**: Calculates the necessary volume for fermentation and primary storage tanks
- **optimize_barrel_rotation**: Suggests a replacement and cleaning schedule to maximize barrel availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Cellar Capacity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many barrels do I need for 5000L of annual production with a 12-month aging regime and a turnover rate of 1.5?"

**🤖 AI Agent:**
> Based on your production of 5000L and a 12-month aging duration, you will need 4000 barrels to satisfy the aging requirements at a 1.5 turnover rate.

---

**👤 You:**
> "What is the required tank capacity for a fermentation volume of 2000L with a peak overlap factor of 1.2?"

**🤖 AI Agent:**
> The required tank volume is 2400L, and you should plan for at least 1 tank based on this requirement.

---

**👤 You:**
> "Show me the seasonal utilization for a production schedule of 1000L every month for a year with 6-month aging."

**🤖 AI Agent:**
> The cellar utilization will steadily increase for the first 6 months as volumes accumulate, reaching a steady state of 6000L total volume in the cellar.


## ❓ FAQ

**Q: How do I calculate the number of barrels I need?**
You can use the `get_barrel_inventory_requirements` tool. Provide your annual production volume, the specific aging regimes for your wines, and your expected barrel turnover rate.

**Q: Can I predict peak cellar usage?**
Yes, the `get_seasonal_space_utilization` tool provides a month-by-month breakdown of volume in the cellar and the percentage of maximum capacity used.

**Q: How can I optimize my barrel cleaning schedule?**
Use the `optimize_barrel_rotation` tool. It suggests a replacement and cleaning schedule designed to align with periods of lowest cellar utilization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-cellar-capacity-planner](https://vinkius.com/ai-agent-connect/wine-cellar-capacity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Cellar Capacity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-cellar-capacity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Cellar Capacity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-cellar-capacity-planner": {
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

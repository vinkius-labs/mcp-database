# Tile Floor Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tile-floor-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate tiles, grout, adhesive, and costs for any floor layout.

## Description
The Tile Floor Calculator is a specialized tool for estimating all necessary installation materials and total expenditures for tiling projects. Whether you are working with simple rectangular rooms or complex, irregular spaces defined by boundary points, this MCP server provides precise estimates. Use `calculate_room_area` to find the surface area of polygonal spaces, `estimate_tile_requirements` to determine tile counts (including waste factors for Straight, Diagonal, or Herringbone patterns) and adhesive amounts, `calculate_joint_and_trim` for grout volume and edge strip lengths, and `sum_project_costs` to finalize your budget based on material unit prices.


## Available Tools (4)
- **calculate_room_area**: Calculate the surface area of a room based on boundary points
- **sum_project_costs**: Calculate the total estimated cost for all materials
- **calculate_joint_and_trim**: Calculate grout volume and edge trim length
- **estimate_tile_requirements**: Estimate the number of tiles and adhesive needed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tile Floor Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the area of a room with corners at (0,0), (10,0), (10,12), and (0,12)?"

**🤖 AI Agent:**
> The total surface area of the room is 120 square units.

---

**👤 You:**
> "I have a floor area of 150 sq ft. How many 12x12 inch tiles do I need for a diagonal pattern?"

**🤖 AI Agent:**
> For a 150 sq ft area using 12x12 inch tiles in a diagonal pattern, you will need approximately 165 tiles (this includes the 10% waste factor).

---

**👤 You:**
> "Calculate grout and trim for a 200 sq ft room with a perimeter of 60 ft, using 1/8 inch joints and 3/8 inch depth."

**🤖 AI Agent:**
> The required grout volume is approximately 0.02 cubic feet, and you will need 60 feet of edge trim.


## ❓ FAQ

**Q: How do I calculate the area for an irregular room?**
You can use the `calculate_room_area` tool by providing a JSON array of `{x, y}` coordinates that represent the vertices or corners of your room's boundary.

**Q: Does the calculator account for tile waste?**
Yes. The `estimate_tile_requirements` tool automatically applies a waste factor based on your chosen pattern: 5% for Straight, 10% for Diagonal, and 15% for Herringbone.

**Q: Can I estimate the total cost of my project?**
Absolutely. Once you have your material quantities from other tools, use `sum_project_costs` with your local unit prices to get a final financial estimate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tile-floor-calculator](https://vinkius.com/mcp/tile-floor-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tile Floor Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tile-floor-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tile Floor Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tile-floor-calculator": {
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

# Floor Material Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/floor-material-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate the exact amount of tiles, wood, or porcelain needed for your flooring project.

## Description
This MCP server provides precise estimation tools for flooring projects. Use `calculate_gross_area` to account for waste, `calculate_tile_effective_area` to include grout width in your coverage calculations, and `calculate_box_count` to determine exactly how many full boxes you need to purchase. It eliminates guesswork by calculating the expanded area based on net dimensions and material wastage patterns.


## Available Tools (3)
- **calculate_tile_effective_area**: Calculates the actual coverage footprint of a single tile or plank, including its grout border
- **calculate_box_count**: Determines the final number of full boxes required to cover the target area
- **calculate_gross_area**: Determines the total surface area that needs to be covered after accounting for cutting and waste


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floor Material Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a room that is 20 square meters and I want to add 10% for waste. What is my total area?"

**🤖 AI Agent:**
> Your total gross area, including the 10% waste margin, is 22 square meters.

---

**👤 You:**
> "If my tile is 30cm by 30cm and the grout is 5mm, what is the effective area per tile?"

**🤖 AI Agent:**
> The effective coverage area for one tile, including the grout width, is 0.093025 square meters.

---

**👤 You:**
> "I need to cover 50 square meters and each box covers 2.5 square meters. How many boxes do I need?"

**🤖 AI Agent:**
> You will need to purchase exactly 20 boxes.


## ❓ FAQ

**Q: How do I account for cutting waste?**
Use the `calculate_gross_area` tool. Provide your net floor area and a waste percentage (e.g., 10 for 10%) to get the total expanded area.

**Q: Does this tool include grout width?**
Yes, by using `calculate_tile_effective_area`, you can input the grout width to find the true coverage footprint of each tile.

**Q: How many boxes should I buy?**
After calculating your total area, use `calculate_box_count` with the manufacturer's box coverage to find the exact number of full boxes required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/floor-material-calculator](https://vinkius.com/mcp/floor-material-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floor Material Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `floor-material-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floor Material Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floor-material-calculator": {
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

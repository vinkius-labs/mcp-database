# Floor Tile Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/floor-tile-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise tile requirements including waste factors.

## Description
This MCP server provides tools to estimate the exact number of tiles needed for any flooring project. It handles area calculations, validates dimensions, suggests waste percentages based on room complexity, and compares different tile sizes to find the most efficient option. Use `get_tile_requirement` to find the total count, `get_standard_waste_recommendation` to determine the buffer for irregular layouts, and `compare_tile_options` to choose between different tile dimensions.


## Available Tools (4)
- **get_standard_waste_recommendation**: Suggests a waste percentage based on the complexity of the floor layout
- **compare_tile_options**: Compares two different tile sizes to determine which one results in less wasted material for a specific area
- **get_tile_requirement**: Calculates the exact number of tiles needed for a specific floor area given tile dimensions and a waste preference
- **validate_area_dimensions**: Checks if the provided floor area and tile dimensions are physically realistic and compatible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floor Tile Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 30x30cm tiles do I need for a 10 square meter floor with 10% waste?"

**🤖 AI Agent:**
> You will need 123 tiles in total.

---

**👤 You:**
> "What is the recommended waste percentage for a room with a diagonal pattern?"

**🤖 AI Agent:**
> A 15% waste factor is recommended for diagonal patterns.

---

**👤 You:**
> "Is a 60x60cm tile more efficient than a 30x30cm tile for a 20sqm area?"

**🤖 AI Agent:**
> The 60x60cm tile is more efficient for this area.


## ❓ FAQ

**Q: How does the tool account for broken tiles?**
The tool uses a waste percentage to add extra tiles to the total, covering breakage and cutting loss.

**Q: Can I compare two different tile sizes?**
Yes, you can use `compare_tile_options` to see which tile size results in less wasted material.

**Q: What if my room has an irregular shape?**
You can use `get_standard_waste_recommendation` to get a suggested waste percentage for irregular layouts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/floor-tile-calculator](https://vinkius.com/en/ai-agent-connect/floor-tile-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floor Tile Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `floor-tile-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floor Tile Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floor-tile-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

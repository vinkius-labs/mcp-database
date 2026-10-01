# Mosaic Tile Layout Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mosaic-tile-layout-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Calculate required tile packages based on design grids and breakage buffers.

## Description
This MCP server provides precise calculations for mosaic tile installations. It allows AI agents to process design grids and determine the exact number of commercial packages needed for each color. By using `get_design_summary`, agents can tally color counts, and with `calculate_required_packages`, they can account for breakage percentages and specific package sizes to generate accurate order lists. It also includes `validate_layout_dimensions` to ensure spatial feasibility.


## Available Tools (4)
- **calculate_required_packages**: Determines the final number of commercial packages to order for every color used in the design
- **get_color_mapping_info**: Retrieves the human-readable names or metadata for the colors used in the design
- **get_design_summary**: Provides a high-level overview of how many tiles of each color are present in the design grid before wastage is applied
- **validate_layout_dimensions**: Ensures the provided tile dimensions are compatible with the grid scale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mosaic Tile Layout Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many tiles of each color are in this grid: [['red', 'blue'], ['blue', 'red']]?"

**🤖 AI Agent:**
> There are 2 red tiles and 2 blue tiles in the design.

---

**👤 You:**
> "Calculate packages for 10 red tiles with 10% breakage and 5 tiles per package."

**🤖 AI Agent:**
> You need to order 3 packages of red tiles.

---

**👤 You:**
> "Is a 10x10 grid with 2x2 tiles valid?"

**🤖 AI Agent:**
> Yes, the dimensions are valid and the total area is 400 square units.


## ❓ FAQ

**Q: How does the tool handle material wastage?**
The `calculate_required_packages` tool applies a breakage percentage to the initial color counts to ensure you have enough tiles to cover cutting and shipping damage.

**Q: Can I verify if my tile dimensions fit my design?**
Yes, you can use the `validate_layout_dimensions` tool to check if your grid rows, columns, and tile dimensions are valid and to calculate the total surface area.

**Q: What information is needed to calculate an order?**
You need the color counts from the design, the breakage percentage, and a mapping of package sizes for each color used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mosaic-tile-layout-counter](https://vinkius.com/en/ai-agent-connect/mosaic-tile-layout-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mosaic Tile Layout Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mosaic-tile-layout-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mosaic Tile Layout Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mosaic-tile-layout-counter": {
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

# 2D Guillotine Packer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/2d-guillotine-packer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Efficiently pack 2D rectangles into a container using the Guillotine split algorithm.

## Description
The 2D Guillotine Packer is a geometric utility designed to determine if a collection of rectangular items can be successfully arranged within a fixed bounding container. Using the efficient Guillotine split algorithm, it manages space by partitioning empty areas into smaller sub-rectangles as items are placed. This tool is ideal for bin-packing problems in UI layout, sprite sheet generation, and material cutting optimization. You can use `pack_rectangles` to find exact coordinates for each item, `calculate_packing_density` to measure area utilization, and `validate_item_compatibility` to perform quick pre-checks on item dimensions.


## Available Tools (3)
- **calculate_packing_density**: Calculates how much of the container's total area is occupied by placed items
- **pack_rectangles**: Determines if a set of 2D rectangles can fit inside a larger bounding rectangle
- **validate_item_compatibility**: Performs a quick pre-check to see if any item's intrinsic size makes it impossible to fit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **2D Guillotine Packer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you pack a 10x10, 5x5, and 2x2 rectangle into a 15x15 container?"

**🤖 AI Agent:**
> Yes, all items can be placed. The 10x10 item is at (0,0), the 5x5 item is at (10,0), and the 2x2 item is at (10,5).

---

**👤 You:**
> "Check if a 20x20 item can fit in a 15x15 container."

**🤖 AI Agent:**
> No, the 20x20 item is too large for the 15x15 container boundaries.

---

**👤 You:**
> "What is the packing density of my current placement?"

**🤖 AI Agent:**
> The calculated packing density for the provided placements within the container is 0.65.


## ❓ FAQ

**Q: How does the packing algorithm work?**
It uses a Guillotine split strategy. The algorithm sorts items by height in descending order and places them into available free rectangles, splitting any remaining space into two new smaller rectangles after each placement.

**Q: Can items be rotated to improve fit?**
Yes, if the `canRotate` property is set to true for an item, the algorithm will attempt to swap its width and height if the original orientation does not fit in a free rectangle.

**Q: What happens if an item cannot fit?**
If any single item in the input list cannot find a suitable free rectangle, the `pack_rectangles` tool returns a failure status and identifies the specific item ID that caused the error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/2d-guillotine-packer](https://vinkius.com/mcp/2d-guillotine-packer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **2D Guillotine Packer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `2d-guillotine-packer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **2D Guillotine Packer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "2d-guillotine-packer": {
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

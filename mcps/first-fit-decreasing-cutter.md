# First-Fit Decreasing Cutter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/first-fit-decreasing-cutter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize material usage by calculating the most efficient cutting plans for raw stock.

## Description
The First-Fit Decreasing Cutter MCP server provides a specialized optimization engine to minimize waste when cutting long materials into smaller pieces. By using the FFD algorithm, it intelligently distributes required pieces across boards to reduce total stock consumption. You can use `calculate_cutting_plan` to generate detailed board breakdowns, `verify_piece_compatibility` to ensure all requested parts fit within your stock length, and `analyze_plan_efficiency` to evaluate waste percentages and utilization rates.


## Available Tools (3)
- **analyze_plan_efficiency**: Evaluates the material waste percentage and utilization rate of a completed cutting plan
- **calculate_cutting_plan**: Determines how to distribute required pieces across multiple boards to minimize total stock consumption
- **verify_piece_compatibility**: Validates whether every requested piece is physically capable of being cut from a single unit of stock


## 💬 Prompt Examples

Here are some examples of how you can interact with the **First-Fit Decreasing Cutter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a cutting plan for a stock length of 3000mm with pieces: 1200mm (A), 1500mm (B), and 800mm (C)."

**🤖 AI Agent:**
> Total boards used: 2. Board 1: Cuts [1500, 1200], Waste: 300mm. Board 2: Cuts [800], Waste: 2200mm.

---

**👤 You:**
> "Check if a 500mm piece is compatible with a 400mm stock length."

**🤖 AI Agent:**
> Incompatible pieces detected: [500mm]. The piece exceeds the available stock length.

---

**👤 You:**
> "Analyze efficiency for 10000mm total stock used with 1500mm total waste."

**🤖 AI Agent:**
> Waste Percentage: 15.0%. Utilization Percentage: 85.0%.


## ❓ FAQ

**Q: How does the optimization algorithm work?**
The engine uses the First-Fit Decreasing (FFD) algorithm. It sorts all required pieces from largest to smallest and then places each piece into the first available board that has enough remaining capacity.

**Q: Can I verify if my pieces are too large for my stock?**
Yes, you can use the `verify_piece_compatibility` tool to check if any piece in your list exceeds the provided stock length.

**Q: What information is included in a cutting plan?**
The `calculate_cutting_plan` tool returns the total number of boards used, the exact sequence of cuts performed on each board, and the remaining waste for every board.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/first-fit-decreasing-cutter](https://vinkius.com/mcp/first-fit-decreasing-cutter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **First-Fit Decreasing Cutter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `first-fit-decreasing-cutter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **First-Fit Decreasing Cutter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "first-fit-decreasing-cutter": {
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

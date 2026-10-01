# Ceramic Firing Shelf Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ceramic-firing-shelf-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimizes kiln shelf layouts by assigning ceramic pieces to available shelves.

## Description
This MCP server automates the complex task of organizing ceramic pieces within a kiln. It uses precise dimensions, required clearances, and stacking limits to calculate the most efficient use of space. Use `plan_shelf_placement` to generate full layouts, `calculate_shelf_capacity` to determine how many items fit on a specific shelf, `find_optimal_shelf` to minimize wasted area, and `validate_stack_integrity` to ensure vertical stacks remain safe during firing.


## Available Tools (4)
- **find_optimal_shelf**: Identifies the most efficient shelf for a specific piece to minimize wasted space
- **plan_shelf_placement**: Generates a detailed layout of where pieces should be placed on available shelves
- **validate_stack_integrity**: Verifies if a proposed stack of ceramic pieces is safe based on height and stacking rules
- **calculate_shelf_capacity**: Determines how many pieces of a specific type can fit on a single shelf given certain constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ceramic Firing Shelf Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you create a placement plan for 5 pieces (10x10x5) on a shelf that is 50x50, with a 2cm clearance and a max stack height of 2?"

**🤖 AI Agent:**
> The pieces have been assigned to shelf ID 'shelf_01' at coordinates (x: 2, y: 2) and (x: 14, y: 2), with one stack of 2 pieces.

---

**👤 You:**
> "How many 5x5cm pieces can fit on a 20x20cm shelf with 1cm clearance and a max stack height of 3?"

**🤖 AI Agent:**
> You can fit a total of 9 pieces on this shelf (3 stacks of 3 pieces each).

---

**👤 You:**
> "Is a stack of three pieces with heights 5cm, 5cm, and 6cm safe if the max stack height is 3?"

**🤖 AI Agent:**
> Yes, the stack is safe because it contains 3 pieces, which does not exceed the maximum stack height of 3.


## ❓ FAQ

**Q: How does the tool handle piece spacing?**
The tool uses the `clearance` parameter to ensure every piece has a mandatory buffer zone around its perimeter to prevent heat interference.

**Q: Can I stack pieces vertically?**
Yes, stacking is supported as long as it does not exceed the `maxStackHeight` and passes the `validate_stack_integrity` check.

**Q: What information do I need to provide?**
You need to provide the dimensions of your shelves, the dimensions of your ceramic pieces, the required clearance, and the maximum stacking height.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ceramic-firing-shelf-planner](https://vinkius.com/en/ai-agent-connect/ceramic-firing-shelf-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ceramic Firing Shelf Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ceramic-firing-shelf-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ceramic Firing Shelf Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ceramic-firing-shelf-planner": {
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

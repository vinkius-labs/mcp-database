# Closet Space Geometry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/closet-space-geometry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate if your clothes will physically fit in your closet based on rail and shelf capacity.

## Description
The Closet Space Geometry Calculator helps you avoid the frustration of overstuffed closets. By analyzing available rail width and shelf surface area against your collection of hangers and folded items, it provides a clear audit of your storage capacity. Use `calculate_rail_load` to check hanger space, `calculate_shelf_load` for folded items, or `generate_capacity_audit` for a complete overview of your closet's health.


## Available Tools (3)
- **generate_capacity_audit**: Generate a summary audit of closet capacity
- **calculate_rail_load**: Calculate if hangers fit on a closet rail
- **calculate_shelf_load**: Calculate if folded items fit on a closet shelf


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Closet Space Geometry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 48 inches of rail space and I want to hang 30 hangers. Each hanger needs 2 inches of width. Will they fit?"

**🤖 AI Agent:**
> No, you need 60 inches of rail for 30 hangers. You must remove 6 hangers to make them fit in your 48-inch space.

---

**👤 You:**
> "Check my shelf capacity: 24 inches wide, 12 inches deep, with 10 folded items that each need 15 square inches of area."

**🤖 AI Agent:**
> Your shelf has 288 square inches available. Your 10 items only require 150 square inches. Everything fits perfectly!

---

**👤 You:**
> "Give me a full audit for a closet that is 40 inches wide and 20 inches deep, with 25 hangers (2 inches each) and 15 folded items (20 square inches each)."

**🤖 AI Agent:**
> You have 40 inches of rail. Your clothes need 50 inches. You must donate 5 items. Additionally, your shelf capacity is exceeded; you need to remove 10 folded items.


## ❓ FAQ

**Q: How does the calculator determine if my clothes will fit?**
It compares the total linear width required by your hangers and the total surface area needed for folded items against the available dimensions of your closet rail and shelves.

**Q: What should I do if the audit shows an overflow?**
The tool returns `itemsToRemove`, specifying exactly how many items you need to remove or donate to bring your closet back within its physical capacity limits.

**Q: Can I use this for both hanging and folded items?**
Yes, you can check them individually using `calculate_rail_load` or `calculate_shelf_load`, or get a combined report with `generate_capacity_audit`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/closet-space-geometry-calculator](https://vinkius.com/mcp/closet-space-geometry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Closet Space Geometry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `closet-space-geometry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Closet Space Geometry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "closet-space-geometry-calculator": {
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

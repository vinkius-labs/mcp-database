# Leftover Inventory Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leftover-inventory-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Track and reuse material offcuts to minimize waste.

## Description
The Leftover Inventory Manager MCP server connects AI agents to your material cutting workflow. It enables the 'Reuse First' principle by tracking offcuts generated during processes like first-fit-decreasing cutting. Use `filter_incoming_waste` to add new pieces to your inventory, `match_requirement_to_offcut` to find the most efficient piece for a specific dimension, and `get_inventory_composition` to audit your current stock by size tier.


## Available Tools (3)
- **filter_incoming_waste**: Filters incoming waste pieces and adds them to inventory
- **get_inventory_composition**: Summarizes the current inventory state
- **match_requirement_to_offcut**: Finds the best offcut for a given requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leftover Inventory Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a new piece needed with length 50mm and width 30mm. Is there an offcut available?"

**🤖 AI Agent:**
> Yes, I found a suitable offcut in your inventory with dimensions 65mm x 40mm.

---

**👤 You:**
> "Add these new waste pieces to my inventory: [{'length': 120, 'width': 50}, {'length': 80, 'width': 40}] with a minimum usable length of 100mm."

**🤖 AI Agent:**
> The piece with 120mm x 50mm was added to the inventory. The piece with 80mm x 40mm was discarded because it is below the 100mm threshold.

---

**👤 You:**
> "What does my current offcut inventory look like?"

**🤖 AI Agent:**
> Your inventory currently contains: 5 Small pieces, 3 Medium pieces, and 2 Large pieces.


## ❓ FAQ

**Q: How does the system decide which pieces to keep?**
The `filter_incoming_waste` tool uses a minimum usable length threshold. Any piece shorter than this value is discarded as true waste.

**Q: How do I find the best piece for a new project?**
Use the `match_requirement_to_offcut` tool. It searches your inventory and selects the piece that satisfies your dimensions while resulting in the least wasted area.

**Q: Can I see a summary of my current stock?**
Yes, the `get_inventory_composition` tool provides a high-level summary of available pieces categorized by Small, Medium, and Large size tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leftover-inventory-manager](https://vinkius.com/mcp/leftover-inventory-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leftover Inventory Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leftover-inventory-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leftover Inventory Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leftover-inventory-manager": {
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

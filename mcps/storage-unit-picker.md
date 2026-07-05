# Storage Unit Picker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/storage-unit-picker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate the required storage unit size based on your items' volume and stacking efficiency.

## Description
The Storage Unit Picker helps you plan your move by determining exactly how much space you need. By selecting common household items, the tool calculates the total cubic footage required, applying a 70% vertical space utilization rule to account for stacking gaps. Use `get_item_catalog` to see available items, `calculate_required_volume` to find the adjusted volume, and `recommend_storage_unit` to match that volume to standard sizes like 5x5, 10x10, or 20x20.


## Available Tools (3)
- **calculate_required_volume**: Determines the total amount of space needed for selected items
- **get_item_catalog**: Retrieves the complete list of all items available for selection
- **recommend_storage_unit**: Matches a volume requirement to the smallest available storage unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storage Unit Picker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a sofa, a refrigerator, and a queen bed set. How much space do I need?"

**🤖 AI Agent:**
> Based on the volumes for a sofa (25 cu ft), refrigerator (30 cu ft), and queen bed set (40 cu ft), your total adjusted volume is approximately 135.71 cubic feet. A 10x10 unit is recommended.

---

**👤 You:**
> "What is the required volume for a standard sofa and a small chair?"

**🤖 AI Agent:**
> The total adjusted volume needed is 42.86 cubic feet, which fits best in a 5x10 storage unit.

---

**👤 You:**
> "Recommend a unit for 300 cubic feet of items."

**🤖 AI Agent:**
> For a requirement of 300 cubic feet, the recommended size is a 10x20 storage unit.


## ❓ FAQ

**Q: How does the volume calculation work?**
The tool sums the cubic feet of all selected items and then increases that total to account for a 70% stacking efficiency, ensuring you don't run out of space due to irregular item shapes.

**Q: What storage unit sizes are considered?**
The tool recommends from standard industry sizes: 5x5, 5x10, 10x10, 10x15, and 10x20.

**Q: How can I see which items are available?**
You can use the `get_item_catalog` tool to retrieve a complete list of common household items and their specific volume requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storage-unit-picker](https://vinkius.com/mcp/storage-unit-picker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storage Unit Picker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `storage-unit-picker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storage Unit Picker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storage-unit-picker": {
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

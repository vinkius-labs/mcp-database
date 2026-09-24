# Sports Jersey Inventory Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sports-jersey-inventory-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Calculate jersey requirements and manage inventory based on team rosters.

## Description
This MCP server provides specialized tools for sports organizations to manage jersey inventory. It allows users to calculate exact jersey needs using `get_required_jersey_count`, assess current stock levels with `get_roster_inventory_summary`, determine team scale tiers via `calculate_team_scale_needs`, and verify storage limits with `validate_order_feasibility`.


## Available Tools (4)
- **validate_order_feasibility**: Checks if a requested jersey order fits within the maximum storage capacity
- **calculate_team_scale_needs**: Determines the team category tier based on the player count
- **get_required_jersey_count**: Calculates the total number of jerseys needed based on player count and spare capacity
- **get_roster_inventory_summary**: Summarizes the relationship between current inventory and required player count


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sports Jersey Inventory Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many jerseys do I need for a team of 25 players with 5 spares?"

**🤖 AI Agent:**
> You will need a total of 30 jerseys.

---

**👤 You:**
> "I have 15 jerseys in stock and 20 players. Do I have enough?"

**🤖 AI Agent:**
> No, you have a shortage of 5 jerseys.

---

**👤 You:**
> "What tier is a team with 150 players?"

**🤖 AI Agent:**
> A team with 150 players is classified as Professional.


## ❓ FAQ

**Q: How does the tool calculate the total number of jerseys needed?**
The `get_required_jersey_count` tool calculates the total by adding the player count to any requested spare capacity for backups.

**Q: Can I check if I have enough jerseys for my current roster?**
Yes, you can use `get_roster_inventory_summary` to compare your current inventory against your player count to identify surpluses or shortages.

**Q: How are team tiers determined?**
Team tiers like Youth, Amateur, or Professional are determined by the player count using the `calculate_team_scale_needs` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sports-jersey-inventory-manager](https://vinkius.com/en/ai-agent-connect/sports-jersey-inventory-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sports Jersey Inventory Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sports-jersey-inventory-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sports Jersey Inventory Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sports-jersey-inventory-manager": {
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

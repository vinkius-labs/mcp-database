# Wine Club Shipment Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-club-shipment-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimizes wine club shipments by matching member preferences with available inventory and price targets.

## Description
This MCP server connects AI agents to wine club logistics. It enables precise shipment planning by analyzing member profiles and real-time inventory. Use `get_member_profiles` to retrieve preferences, `get_available_inventory` to check stock, `optimize_shipment_plan` to generate the best wine mix, and `validate_shipment_feasibility` to ensure plans meet tier and budget constraints.


## Available Tools (4)
- **optimize_shipment_plan**: Generates the optimal wine selection for all members based on constraints
- **validate_shipment_feasibility**: Checks if a proposed shipment plan is physically and financially possible
- **get_available_inventory**: You can choose to include exclusive wines.

Provides a real-time snapshot of current wine stock, including quality and exclusivity status
- **get_member_profiles**: Retrieves detailed preference profiles and historical satisfaction data for all club members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Club Shipment Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the preferences for members in the Reserve tier?"

**🤖 AI Agent:**
> Members in the Reserve tier generally prefer premium varietals like Cabernet Sauvignon and Chardonnay, with a moderate price range preference.

---

**👤 You:**
> "Generate a shipment plan that maximizes member satisfaction within a $500 to $1000 price range."

**🤖 AI Agent:**
> The optimized shipment plan has been generated, selecting a mix of premium varietals that maximizes satisfaction while staying within the $500-$1000 range for all targeted members.

---

**👤 You:**
> "Is there any Cabernet Sauvignon available in the inventory?"

**🤖 AI Agent:**
> Yes, there are currently 45 units of Cabernet Sauvignon available in the inventory.


## ❓ FAQ

**Q: How does the optimizer handle exclusive wines?**
The `optimize_shipment_plan` tool respects tier access levels, ensuring exclusive wines are only assigned to members in the Icon tier.

**Q: Can I check if a shipment plan is valid?**
Yes, use the `validate_shipment_feasibility` tool to check for inventory shortages, price violations, or tier mismatches.

**Q: How do I see what wines are currently in stock?**
You can use `get_available_inventory` to see a real-time snapshot of current wine stock and exclusivity status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-club-shipment-optimizer](https://vinkius.com/en/ai-agent-connect/wine-club-shipment-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Club Shipment Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-club-shipment-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Club Shipment Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-club-shipment-optimizer": {
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

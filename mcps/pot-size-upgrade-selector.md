# Pot Size Upgrade Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pot-size-upgrade-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Selects compatible pot sizes based on plant root mass, height, and desired clearance.

## Description
This MCP server helps users select the ideal container for plant transplantation. By analyzing the current root-ball width, plant height, and requested clearance, it identifies compatible pots from the catalog. It uses `get_compatible_pots` to find suitable matches, `rank_pot_options` to prioritize them for stability and growth, and `check_inventory_availability` to ensure the selected items are in stock. It also provides `calculate_growth_capacity` to estimate the available room for new root development.


## Available Tools (4)
- **calculate_growth_capacity**: Estimates the potential growth room provided by a specific pot selection
- **check_inventory_availability**: Filters a list of potential pot sizes against the current stock levels
- **get_compatible_pots**: Identifies all available pot sizes that meet the minimum physical requirements for a specific plant
- **rank_pot_options**: Sorts the compatible pots into a prioritized list based on optimal growth room and stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pot Size Upgrade Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me some pots for a plant with a 10cm root-ball width and I want 5cm of clearance. The plant is 30cm tall."

**🤖 AI Agent:**
> I found three compatible pots. The best option is the Standard Growth Pot (ID: pot-std-02) with a 16cm diameter, which provides the exact 5cm clearance you requested while maintaining excellent stability for a 30cm plant.

---

**👤 You:**
> "What is the growth capacity for a 12cm diameter pot with 500ml volume for my plant with a 10cm root-ball?"

**🤖 AI Agent:**
> The pot provides a diameter buffer of 2cm and a volume ratio of 1.4 relative to the current root mass.

---

**👤 You:**
> "Are the large specimen pots currently available in stock?"

**🤖 AI Agent:**
> The Large Specimen Pot (ID: pot-spec-01) is currently in stock and available for selection.


## ❓ FAQ

**Q: How does the tool determine if a pot is compatible?**
A pot is considered compatible if its internal diameter is strictly greater than the sum of the current root-ball width and the requested clearance.

**Q: How are the pot recommendations ranked?**
Pots are ranked by balancing the requested clearance with stability requirements. The tool avoids recommending excessively large pots that might cause over-watering issues.

**Q: Can I check if a specific pot is in stock?**
Yes, the tool includes functionality to check real-time inventory availability for specific pot IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pot-size-upgrade-selector](https://vinkius.com/en/ai-agent-connect/pot-size-upgrade-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pot Size Upgrade Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pot-size-upgrade-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pot Size Upgrade Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pot-size-upgrade-selector": {
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

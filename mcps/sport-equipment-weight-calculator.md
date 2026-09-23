# Sport Equipment Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sport-equipment-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate total mass and validate load capacity for athletic equipment sets.

## Description
This MCP server provides tools to manage and calculate the cumulative mass of athletic equipment. Use `get_equipment_catalog` to browse available gear, `calculate_set_weight` to sum the total mass of specific items, and `validate_load_capacity` to ensure equipment sets do not exceed safety limits for transport or storage. It also includes `search_equipment_by_weight_range` to find gear within specific weight constraints.


## Available Tools (4)
- **calculate_set_weight**: Calculate the total weight of a selection of equipment
- **get_equipment_catalog**: Retrieve the catalog of available athletic equipment
- **search_equipment_by_weight_range**: Search for equipment within a specific weight range
- **validate_load_capacity**: Check if a set of equipment exceeds a weight limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sport Equipment Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total weight of the equipment with IDs 'barbell_01' and 'plate_05'?"

**🤖 AI Agent:**
> The total weight for those items is 45 kg.

---

**👤 You:**
> "Is it safe to carry a set of equipment weighing 50kg if my limit is 40kg?"

**🤖 AI Agent:**
> No, the current weight is 50 kg, which exceeds your 40 kg limit by 10 kg.

---

**👤 You:**
> "Show me all equipment that weighs less than 2kg."

**🤖 AI Agent:**
> The available items under 2kg are: Jump Rope (0.2kg) and Resistance Band (0.5kg).


## ❓ FAQ

**Q: How can I see what equipment is available?**
You can use the `get_equipment_catalog` tool to retrieve a full list of available items and their weights.

**Q: Can I check if my gym bag can hold all my gear?**
Yes, use the `validate_load_capacity` tool by providing the equipment IDs and the maximum weight capacity of your bag.

**Q: How do I find light equipment?**
Use the `search_equipment_by_weight_range` tool and set a `maxWeight` value to find items within your desired range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sport-equipment-weight-calculator](https://vinkius.com/en/ai-agent-connect/sport-equipment-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sport Equipment Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sport-equipment-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sport Equipment Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sport-equipment-weight-calculator": {
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

# Moving Truck Load Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-truck-load-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Optimize truck cargo space and weight distribution for safe transport.

## Description
This MCP server provides specialized tools for logistics and moving operations. It allows AI agents to retrieve truck capacities using `get_truck_capacity`, generate optimized loading plans with `plan_load_configuration`, verify loading sequences via `validate_loading_order`, and ensure vehicle stability with `calculate_center_of_gravity`. It helps manage weight limits, volume constraints, and loading order dependencies to ensure safe and efficient cargo transport.


## Available Tools (4)
- **calculate_center_of_gravity**: Determines if the planned load distribution is safe for transport
- **get_truck_capacity**: Retrieves the static physical and weight limits of a specific truck model
- **plan_load_configuration**: Generates a loading plan based on a list of items and truck constraints
- **validate_loading_order**: Checks if a proposed loading sequence adheres to the specified dependency constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Truck Load Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum weight capacity for the 'heavy-duty-01' truck model?"

**🤖 AI Agent:**
> The 'heavy-duty-01' truck model has a maximum weight capacity of 15,000 kg and a maximum volume of 60 cubic meters.

---

**👤 You:**
> "Plan a load for truck 'medium-van-02' with these items: item_1 (50kg, 1x1x1m), item_2 (200kg, 2x1x1m)."

**🤖 AI Agent:**
> The load plan for 'medium-van-02' has been generated. Items item_1 and item_2 are assigned to the Front and Middle load zones. Total weight used is 250kg with 150kg remaining.

---

**👤 You:**
> "Is the sequence [item_2, item_1] valid if item_1 must be loaded before item_2?"

**🤖 AI Agent:**
> No, the sequence is invalid because the constraint requires item_1 to be loaded before item_2.


## ❓ FAQ

**Q: How can I check if a truck can hold my items?**
You can use the `get_truck_capacity` tool to find the limits of a specific truck model, and then use `plan_load_configuration` to see if your items fit within those limits.

**Q: Can I enforce specific loading orders?**
Yes, the `plan_load_configuration` tool accepts loading constraints to ensure items are loaded in the correct sequence, and `validate_loading_order` can verify your proposed sequence.

**Q: How is vehicle stability ensured?**
The `calculate_center_of_gravity` tool analyzes the distribution of items across load zones to determine if the load is safe and stable for transport.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-truck-load-planner](https://vinkius.com/en/ai-agent-connect/moving-truck-load-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Truck Load Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-truck-load-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Truck Load Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-truck-load-planner": {
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

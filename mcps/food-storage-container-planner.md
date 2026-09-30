# Food Storage Container Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-storage-container-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes meal prep by matching food portions to the best available storage containers.

## Description
This MCP server helps organize meal-prepped food by matching cooked portions to physical containers. It uses tools like `find_optimal_container` to select the smallest suitable vessel, `query_available_containers` to browse your inventory, and `validate_meal_plan` to ensure your storage plan fits within your fridge capacity and respects microwave safety requirements. It also provides insights into fridge space usage via `calculate_fridge_utilization`.


## Available Tools (4)
- **calculate_fridge_utilization**: Calculates how much of the available refrigerator space is being used by a specific set of containers
- **find_optimal_container**: Finds the best single container for a specific food portion
- **query_available_containers**: Retrieves a list of all available storage containers to check their properties
- **validate_meal_plan**: Checks if a proposed set of food-to-container assignments is physically possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Storage Container Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best container for a 500ml portion of pasta that needs to be microwaved."

**🤖 AI Agent:**
> The best container is the Specialty Tier container (ID: cont_99) with a 550ml compartment.

---

**👤 You:**
> "What containers are available if I have 2000ml of fridge space left?"

**🤖 AI Agent:**
> There are 5 containers available that fit within your 2000ml limit: 2 Standard Tier and 3 Single Tier containers.

---

**👤 You:**
> "Is my meal plan valid? I have assigned a 300ml portion to container 'c1' (compartment 0) and a 400ml portion to 'c2' (compartment 0), with a total fridge capacity of 1000ml."

**🤖 AI Agent:**
> Yes, the plan is valid. The total volume used is within the 1000ml limit and all portions fit their compartments.


## ❓ FAQ

**Q: How does the tool select a container?**
The `find_optimal_container` tool selects the smallest container that can fit the food volume, satisfies microwave safety needs, and fits within your remaining fridge capacity.

**Q: Can I validate my entire meal plan at once?**
Yes, you can use `validate_meal_plan` to check if all your assignments are physically possible based on container volumes and fridge limits.

**Q: How do I know if my fridge is full?**
You can use `calculate_fridge_utilization` to see the percentage of space used by your currently assigned containers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-storage-container-planner](https://vinkius.com/en/ai-agent-connect/food-storage-container-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Storage Container Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-storage-container-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Storage Container Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-storage-container-planner": {
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

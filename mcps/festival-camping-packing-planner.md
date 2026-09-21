# Festival Camping Packing Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/festival-camping-packing-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate deterministic festival packing plans with weight, volume, and group sharing optimization.

## Description
This MCP server provides a suite of tools to prepare for camping trips and music festivals. It calculates precise packing requirements based on duration, weather ranges, and campsite rules. Use `generate_packing_plan` to create a full summary including weight and volume, `validate_item_compliance` to check against prohibited items, `calculate_consumable_requirements` for food and water needs, and `optimize_group_sharing` to distribute the load among group members.


## Available Tools (4)
- **calculate_consumable_requirements**: Determines the baseline amount of food and water needed for a specific duration and temperature
- **generate_packing_plan**: Creates a comprehensive, deterministic packing list and summary for an individual or a group
- **optimize_group_sharing**: Recommends how to split the load among group members to minimize individual weight
- **validate_item_compliance**: Checks if a specific item or set of items adheres to the campsite's specific rules and constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Festival Camping Packing Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 3-night camping trip for 2 people. Min temp is 10C, max is 25C. Rules: No gas canisters. Items: Tent (shared), Sleeping Bag, Water Bottle."

**🤖 AI Agent:**
> Total weight: 8.5kg. Total volume: 15L. Missing essentials: Stove, Food. Prohibited items: Gas canisters. Per-person allocation: Person A carries the Tent and Sleeping Bag; Person B carries the Water Bottle.

---

**👤 You:**
> "How much water do 4 people need for 2 nights if the max temperature is 30C?"

**🤖 AI Agent:**
> You will need 24 liters of water for 4 people over 2 nights at 30C.

---

**👤 You:**
> "Check if these items are compliant: [{"name": "Gas Stove", "category": "Kitchen"}] with rule 'No gas canisters'."

**🤖 AI Agent:**
> The item 'Gas Stove' is prohibited based on the rule 'No gas canisters'.


## ❓ FAQ

**Q: How does the planner handle group trips?**
You can use `optimize_group_sharing` to distribute items among participants, ensuring shared items like tents are split efficiently to minimize individual weight.

**Q: Can I check if my gear is allowed at a specific festival?**
Yes, the `validate_item_compliance` tool checks your items against the specific campsite rules you provide to identify any prohibited gear.

**Q: Does it account for weather changes?**
Yes, the `generate_packing_plan` tool uses the minimum and maximum temperature ranges to identify missing essentials like thermal gear or hydration supplies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/festival-camping-packing-planner](https://vinkius.com/en/ai-agent-connect/festival-camping-packing-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Festival Camping Packing Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `festival-camping-packing-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Festival Camping Packing Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "festival-camping-packing-planner": {
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

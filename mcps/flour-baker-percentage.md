# Flour Baker Percentage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flour-baker-percentage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate ingredient baker percentages and scale recipes accurately.

## Description
This MCP server provides professional baking tools to manage ingredient ratios using the Baker's Percentage method. It allows you to calculate the percentage of an ingredient relative to flour weight using `calculate_ingredient_percentage`, determine required ingredient weights with `calculate_ingredient_weight`, scale entire recipes using `batch_scale_recipe`, and verify hydration levels with `validate_hydration_levels`.


## Available Tools (4)
- **calculate_ingredient_percentage**: Calculates the baker's percentage for a single ingredient based on its weight and the total flour weight
- **calculate_ingredient_weight**: Determines the required weight of an ingredient when the baker's percentage and total flour weight are known
- **batch_scale_recipe**: Scales an entire set of ingredient percentages to a new total flour weight
- **validate_hydration_levels**: Checks if the water content in a recipe falls within standard professional ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flour Baker Percentage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I have 500g of flour and 350g of water, what is the water percentage?"

**🤖 AI Agent:**
> The water percentage is 70%.

---

**👤 You:**
> "I need 450g of salt for a recipe where the flour is 1000g. What is the salt percentage?"

**🤖 AI Agent:**
> The salt percentage is 45%.

---

**👤 You:**
> "Scale a recipe with 60% water and 2% salt to a new flour weight of 1200g."

**🤖 AI Agent:**
> The scaled weights are 720g for water and 24g for salt.


## ❓ FAQ

**Q: What is Baker's Percentage?**
Baker's Percentage is a method where the weight of the flour is always 100%, and all other ingredients are expressed as a percentage of that flour weight.

**Q: How do I scale a recipe for a larger batch?**
You can use the `batch_scale_recipe` tool to provide your existing ingredient percentages and a new target flour weight to get the updated ingredient weights.

**Q: Can I check if my dough hydration is correct?**
Yes, the `validate_hydration_levels` tool checks if your water percentage falls within your specified minimum and maximum hydration ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flour-baker-percentage](https://vinkius.com/en/ai-agent-connect/flour-baker-percentage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flour Baker Percentage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flour-baker-percentage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flour Baker Percentage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flour-baker-percentage": {
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

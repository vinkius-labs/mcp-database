# Hobby Supply Shopping Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hobby-supply-shopping-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize hobby project procurement by balancing material needs, budget, and existing tool inventory.

## Description
This MCP server acts as a specialized procurement assistant for hobbyists. It connects AI agents to your project requirements and inventory to ensure you only buy what is necessary. Use `get_project_requirements` to see what a project needs, `check_user_inventory` to see what you already own, and `calculate_shopping_list` to generate a budget-optimized purchase plan. You can also use `simulate_shipping_impact` to compare different shipping tiers like standard, express, or economy.


## Available Tools (4)
- **calculate_shopping_list**: Generates a list of items that need to be purchased by comparing project requirements against user inventory and budget
- **check_user_inventory**: Identifies which reusable tools the user already owns
- **get_project_requirements**: Retrieves the specific list of materials and tools needed to complete a defined project
- **simulate_shipping_impact**: Evaluates how different shipping options or vendor groupings affect the total project cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hobby Supply Shopping Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to start a Miniature Painting Starter project. My budget is $50 and my user ID is user_123. What should I buy?"

**🤖 AI Agent:**
> To complete the Miniature Painting Starter project within your $50 budget, you need to purchase 2 sets of acrylic paints and 1 fine-tip brush. The total estimated cost including shipping is $42.50.

---

**👤 You:**
> "What tools do I need for Basic Woodworking?"

**🤖 AI Agent:**
> The Basic Woodworking project requires a hand saw, a set of clamps, a measuring tape, and sandpaper.

---

**👤 You:**
> "How much will it cost to ship my hobby supplies using express shipping?"

**🤖 AI Agent:**
> Using express shipping for your current shopping list will result in a shipping cost of $15.00, bringing your final total to $65.00.


## ❓ FAQ

**Q: How does the tool prevent me from buying tools I already own?**
The `calculate_shopping_list` tool compares the project requirements against your current inventory using `check_user_inventory` to ensure only missing tools are added to the list.

**Q: Can I plan for projects that exceed my budget?**
Yes. If the total cost exceeds your `maxBudget`, the tool will still provide a prioritized list of necessary items, but the `isWithinBudget` flag will be set to false.

**Q: Does the tool account for shipping costs?**
Yes, the total estimated cost includes a standard shipping fee. You can also use `simulate_shipping_impact` to evaluate how different shipping methods affect your final total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hobby-supply-shopping-planner](https://vinkius.com/en/ai-agent-connect/hobby-supply-shopping-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hobby Supply Shopping Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hobby-supply-shopping-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hobby Supply Shopping Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hobby-supply-shopping-planner": {
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

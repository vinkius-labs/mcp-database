# Pet Food Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-food-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise pet food quantities and costs for weekly, monthly, and annual budgets.

## Description
This MCP server provides a suite of tools to help pet owners manage their food expenses. By providing details like daily portion size, feeding frequency, and package weight, you can use `calculate_feeding_needs` to determine total daily requirements. You can then use `estimate_package_usage` and `calculate_budget_totals` to project costs over weeks, months, or a full year. Finally, `get_shopping_list` ensures you know exactly how many full packages to buy to avoid running out of food.


## Available Tools (4)
- **calculate_budget_totals**: Provides a complete financial overview for weekly, monthly, and annual periods
- **calculate_feeding_needs**: Determines the total weight of food required per day for all pets
- **estimate_package_usage**: Calculates how many full or partial packages are required to meet feeding needs
- **get_shopping_list**: Generates the exact number of whole packages to purchase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Food Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much food and money will I need for 2 dogs that eat 500g twice a day, using 2kg bags that cost $15, with a 5% waste allowance?"

**🤖 AI Agent:**
> For 2 dogs, you will need approximately 2.1kg of food per day. This results in a weekly requirement of 14.7kg and an annual requirement of 766.5kg. You should purchase 8 bags per week or 384 bags per year, with an estimated annual cost of $5,760.

---

**👤 You:**
> "I have 1 cat eating 50g three times a day. The food comes in 500g bags for $10. How many bags do I need for a month?"

**🤖 AI Agent:**
> You will need 150g of food per day. For a standard month (30.44 days), you will need approximately 4.57kg of food, which requires purchasing 10 bags.

---

**👤 You:**
> "Calculate the annual budget for a pet eating 1kg of food daily, with 1kg bags costing $5."

**🤖 AI Agent:**
> The annual food requirement is 365kg. At $5 per 1kg bag, your total annual budget will be $1,825.


## ❓ FAQ

**Q: How does the tool account for food waste?**
You can use the `calculate_feeding_needs` tool with the `wastePercentage` parameter to add a buffer for spills or spoilage.

**Q: Can I calculate costs for multiple pets at once?**
Yes, simply provide the total number of animals in the `numberOfPets` field when using `calculate_feeding_needs`.

**Q: Does this tool provide veterinary advice?**
No, this tool is strictly for financial and quantity budgeting. Always consult a veterinarian for nutritional or feeding recommendations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-food-budget-planner](https://vinkius.com/en/ai-agent-connect/pet-food-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Food Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-food-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Food Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-food-budget-planner": {
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

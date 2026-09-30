# Weekly Grocery Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-grocery-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate optimized grocery lists by reconciling meal needs with pantry stock and budget.

## Description
This MCP server acts as a smart planning engine that bridges your AI assistant to your kitchen management. It calculates exactly what you need to buy by comparing planned meals against your current pantry stock. Using `calculate_net_requirements`, it determines the raw ingredient needs, while `optimize_grocery_list` converts those needs into a realistic shopping list based on real-world package sizes and your budget. If items are too expensive, `suggest_substitutions` provides culinary alternatives to keep you within budget. It is designed to work with Cursor, VS Code, Claude Desktop, and Windsurf via Vinkius Edge.


## Available Tools (4)
- **calculate_net_requirements**: Determines the raw amount of ingredients needed after accounting for what the user already has
- **get_meal_details**: Retrieves the ingredient breakdown for a specific meal
- **optimize_grocery_list**: Converts raw ingredient needs into a realistic shopping list based on package sizes and budget
- **suggest_substitutions**: Provides alternative ingredient options when a primary ingredient is too expensive or unavailable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Grocery Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to plan meals for 4 people. I have 200g of flour in my pantry. What do I need to buy for a pasta meal?"

**🤖 AI Agent:**
> To serve 4 people, you need 500g of flour. After accounting for your 200g pantry stock, you need to buy one 500g bag of flour.

---

**👤 You:**
> "My budget is $20. Can you optimize my grocery list for these meals?"

**🤖 AI Agent:**
> Your optimized list totals $18.50, leaving $1.50 remaining in your budget.

---

**👤 You:**
> "What are some alternatives for salmon if it is too expensive?"

**🤖 AI Agent:**
> Good alternatives for salmon include trout or arctic char, which may be more budget-friendly.


## ❓ FAQ

**Q: How does the tool handle my existing food?**
The `calculate_net_requirements` tool subtracts your current pantry stock from the total ingredients needed for your meals, ensuring you only buy what you actually lack.

**Q: What happens if my grocery list exceeds my budget?**
The `optimize_grocery_list` tool attempts to stay within your budget. If it cannot, it identifies shortages and you can use `suggest_substitutions` to find cheaper alternatives.

**Q: Does it suggest specific package sizes?**
Yes, the `optimize_grocery_list` tool uses a package catalog to suggest buying full packages (like a 500g bag) rather than just raw weights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-grocery-plan](https://vinkius.com/en/ai-agent-connect/weekly-grocery-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Grocery Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-grocery-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Grocery Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-grocery-plan": {
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

# Clothing Capsule Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/clothing-capsule-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Build a cohesive wardrobe by identifying gaps and generating optimized shopping plans.

## Description
This MCP server helps you build a perfect clothing capsule. Use `get_wardrobe_summary` to see what you already own, then use `analyze_wardrobe_gaps` to find what is missing for upcoming occasions. Finally, `generate_shopping_plan` creates a prioritized list of items that fit your budget, while `validate_color_cohesion` ensures every new piece matches your existing style.


## Available Tools (4)
- **generate_shopping_plan**: Creates a prioritized list of items to purchase that satisfies the gaps while staying within the user's budget
- **get_wardrobe_summary**: Provides a high-level overview of what the user currently owns
- **validate_color_cohesion**: Checks if a proposed new item will mathematically increase the versatility of the current wardrobe
- **analyze_wardrobe_gaps**: Identifies which specific items are missing to satisfy a set of upcoming occasions and seasonal needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clothing Capsule Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What do I have in my wardrobe right now?"

**🤖 AI Agent:**
> You currently own 5 items: 2 white t-shirts, 1 pair of blue denim jeans, 1 black sweater, and 1 navy blazer.

---

**👤 You:**
> "I need to dress for a business formal event this winter. What am I missing?"

**🤖 AI Agent:**
> To meet business formal requirements for winter, you are missing a charcoal wool suit and a pair of black leather dress shoes.

---

**👤 You:**
> "Create a shopping plan for my gaps with a budget of $200."

**🤖 AI Agent:**
> Your shopping plan includes a beige trench coat ($120) and a white button-down shirt ($50), totaling $170.


## ❓ FAQ

**Q: How do I start planning my wardrobe?**
Start by calling `get_wardrobe_summary` to provide the agent with a clear view of your current collection.

**Q: Can I plan for specific seasons?**
Yes, use `analyze_wardrobe_gaps` and specify the `targetSeason` to find items appropriate for that time of year.

**Q: How does the budget constraint work?**
When using `generate_shopping_plan`, the agent will prioritize items that satisfy your needs while ensuring the total cost stays within your specified budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/clothing-capsule-planner](https://vinkius.com/en/ai-agent-connect/clothing-capsule-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clothing Capsule Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clothing-capsule-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clothing Capsule Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clothing-capsule-planner": {
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

# Potluck Portion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/potluck-portion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Divide food portions evenly among dishes while respecting dietary constraints.

## Description
The Potluck Portion Calculator is an automated distribution engine designed to manage food quantities for any gathering. It ensures that every guest is fed by calculating how many portions should be allocated to each dish. You can use `calculate_even_distribution` to split portions equally, `filter_by_dietary_needs` to find specific food types, or `optimize_distribution_with_constraints` to ensure dietary requirements like vegan or gluten-free needs are met by specific dishes. It also provides a high-level overview of your food variety using `get_dish_summary`.


## Available Tools (4)
- **calculate_even_distribution**: Determines how many portions should be allocated to each dish to meet the target number of portions
- **filter_by_dietary_needs**: Identifies which subset of dishes can satisfy specific dietary requirements
- **get_dish_summary**: Provides a high-level overview of the total capacity and variety of the potluck
- **optimize_distribution_with_constraints**: Calculates a distribution where specific dishes are reserved for specific dietary needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Potluck Portion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 20 portions to distribute among 3 dishes: Salad, Pasta, and Fruit. How many portions per dish?"

**🤖 AI Agent:**
> Each dish should receive 6 portions, with a remainder of 2 portions.

---

**👤 You:**
> "Find all vegan dishes from this list: [{"id": "1", "name": "Vegan Salad", "dietaryTags": ["vegan"]}, {"id": "2", "name": "Beef Stew", "dietaryTags": ["meat"]}]."

**🤖 AI Agent:**
> The compatible dish is Vegan Salad.

---

**👤 You:**
> "Give me a summary of these dishes: [{"id": "1", "name": "Tacos", "dietaryTags": ["gluten-free"]}, {"id": "2", "name": "Cake", "dietaryTags": ["sweet"]}]."

**🤖 AI Agent:**
> There are 2 dishes with 2 unique dietary tags. The capacity estimate is 2 portions.


## ❓ FAQ

**Q: How does the tool handle leftovers?**
The tool calculates a remainder, which represents the leftover portions that could not be distributed as whole numbers across the dishes.

**Q: Can I ensure vegan guests get enough food?**
Yes, you can use `optimize_distribution_with_constraints` to reserve specific dishes for dietary tags like vegan or gluten-free.

**Q: What happens if I provide no dishes?**
The tool will return an error if the list of dishes provided is empty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/potluck-portion-calculator](https://vinkius.com/en/ai-agent-connect/potluck-portion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Potluck Portion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `potluck-portion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Potluck Portion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "potluck-portion-calculator": {
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

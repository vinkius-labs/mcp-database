# Wedding Budget Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Intelligently distribute wedding funds across categories based on priorities and limits.

## Description
This MCP server provides a suite of tools to manage wedding finances. Use `allocate_budget` to distribute a total budget across essential categories like venue, food, and decor based on your specific priorities and spending limits. You can also use `get_category_summary` to inspect individual category details, `calculate_per_guest_impact` to see how guest counts affect your spending, and `validate_budget_integrity` to ensure your plan follows all constraints.


## Available Tools (4)
- **allocate_budget**: Calculates the distribution of funds across all wedding categories
- **calculate_per_guest_impact**: Analyzes how changes in guest count affect the available budget per person
- **get_category_summary**: Provides a detailed breakdown of a specific category's allocation
- **validate_budget_integrity**: Checks if the current allocation adheres to all constraints and business rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Budget Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Allocate a $20,000 budget for 100 guests. Prioritize Food and Venue highly, and set a $2,000 limit for Flowers."

**🤖 AI Agent:**
> The budget has been allocated. Venue: $7,000, Food: $6,000, Beverage: $2,000, Attire: $1,000, Photography: $1,500, Music: $500, Decor: $500, Flowers: $2,000, Transport: $500, Guests: $0, Taxes: $0, Contingency: $0. Per-guest cost is $200.

---

**👤 You:**
> "How much will my per-guest cost change if I increase my guest count from 100 to 120 with a $20,000 budget?"

**🤖 AI Agent:**
> Increasing the guest count to 120 reduces your current per-guest cost from $200 to $166.67.

---

**👤 You:**
> "Show me the details for the Food category from my allocation."

**🤖 AI Agent:**
> The Food category has been allocated $6,000 with no specific limit set.


## ❓ FAQ

**Q: How does the budget allocation work?**
The `allocate_budget` tool distributes funds by following your priority ranking. It fills higher priority categories first until they reach their limit or the total budget is used.

**Q: Can I set maximum spending limits for specific categories?**
Yes, when using `allocate_budget`, you can provide a limits object to set hard ceilings on specific categories.

**Q: How do I check if my budget plan is valid?**
You can use the `validate_budget_integrity` tool to check if your allocation is consistent and adheres to all set limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator](https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Budget Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-budget-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Budget Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-budget-allocator": {
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

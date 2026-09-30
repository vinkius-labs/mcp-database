# Shared Gift Shopping Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shared-gift-shopping-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Coordinates group gift buying by optimizing selection based on recipient profiles, budgets, and shipping deadlines.

## Description
This MCP server acts as a coordination engine for group gift buying. It helps teams and families select the perfect gift by analyzing recipient preferences, calculating total contribution pools, and validating shipping logistics. Use `get_recipient_preferences` to understand what a recipient likes, `calculate_available_budget` to sum up contributions, and `validate_logistics` to ensure the gift arrives on time. Finally, `generate_gift_plan` provides a complete recommendation that fits both the budget and the delivery deadline.

### Available Tools

`get_recipient_preferences_tool`, `calculate_available_budget_tool`, `validate_logistics_tool`, `generate_gift_plan_tool`


## Available Tools (4)
- **calculate_available_budget_tool**: Determines the total amount of money available for purchasing gifts
- **generate_gift_plan_tool**: Recommends a gift selection that satisfies the recipient's tastes and stays within financial and temporal bounds
- **get_recipient_preferences_tool**: Retrieves the profile of a specific recipient to understand what they like and dislike
- **validate_logistics_tool**: Checks if a specific shipping method and purchase timing are feasible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shared Gift Shopping Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a gift for recipient 'user_123' with a total budget of $100. The gift must arrive by 2024-12-25 and shipping takes 5 days."

**🤖 AI Agent:**
> The suggested gift is a Premium Coffee Maker kit for $85.00. It is expected to arrive on 2024-12-20, which fits your budget and the deadline.

---

**👤 You:**
> "Calculate the total budget if the contributions are 20, 30, and 50."

**🤖 AI Agent:**
> The total available budget is $100.00, with an average contribution of $33.33.

---

**👤 You:**
> "Check if I can buy a gift on 2024-11-01 with a 10-day shipping time for a deadline of 2024-11-15."

**🤖 AI Agent:**
> Yes, the delivery is feasible. The estimated arrival date is 2024-11-11, providing a 4-day buffer before the deadline.


## ❓ FAQ

**Q: How does the tool ensure the gift arrives on time?**
The `validate_logistics` tool checks the purchase date and shipping lead time against the required deadline to ensure the delivery is feasible. Tools available: `get_recipient_preferences_tool`, `calculate_available_budget_tool`, `validate_logistics_tool`.

**Q: Can I use this to manage a budget for multiple people?**
Yes, you can use `calculate_available_budget` to determine the total pool of money collected from all participants.

**Q: What happens if no gift fits the budget?**
If no gift satisfies the recipient's interests while staying within the budget and timeline, the `generate_gift_plan` tool will return an error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shared-gift-shopping-plan](https://vinkius.com/en/ai-agent-connect/shared-gift-shopping-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shared Gift Shopping Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shared-gift-shopping-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shared Gift Shopping Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shared-gift-shopping-plan": {
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

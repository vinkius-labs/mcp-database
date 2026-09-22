# Hobby Budget Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hobby-budget-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and analyze expenses for your personal hobbies.

## Description
Manage your hobby spending with precision. This MCP server allows you to monitor total costs, check if you are staying within your budget, and analyze how quickly you are spending money. Use `get_hobby_total` to see cumulative costs, `check_budget_status` to monitor limits, `calculate_spending_velocity` to track daily spending rates, and `list_hobby_expenses` to view individual transactions.


## Available Tools (4)
- **check_budget_status**: Check if the spending for a hobby is within the budget limit
- **get_hobby_total**: Get the total amount spent on a specific hobby
- **list_hobby_expenses**: List all individual expenses for a specific hobby
- **calculate_spending_velocity**: Calculate the average daily spending rate for a hobby


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hobby Budget Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much have I spent on Photography in total?"

**🤖 AI Agent:**
> You have spent a total of $450.00 on Photography.

---

**👤 You:**
> "Am I over my $200 budget for Gardening?"

**🤖 AI Agent:**
> No, you have $50.00 remaining in your Gardening budget.

---

**👤 You:**
> "What is my daily spending rate for Gaming over the last 7 days?"

**🤖 AI Agent:**
> Your average daily spend for Gaming over the last 7 days is $12.50.


## ❓ FAQ

**Q: How can I see my total spending for a specific hobby?**
You can use the `get_hobby_total` tool to retrieve the total amount spent on any hobby you specify.

**Q: Can I set a budget limit?**
Yes, use the `check_budget_status` tool to compare your current spending against a defined budget limit.

**Q: How do I see a list of my purchases?**
The `list_hobby_expenses` tool provides a detailed list of all individual items purchased for your hobby.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hobby-budget-tracker](https://vinkius.com/en/ai-agent-connect/hobby-budget-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hobby Budget Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hobby-budget-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hobby Budget Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hobby-budget-tracker": {
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

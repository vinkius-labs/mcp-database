# Wellness Expense Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-expense-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Monitor and analyze your wellness-specific spending patterns.

## Description
This MCP server provides specialized tools to track and analyze wellness-related expenses. Use `get_spending_summary` to see a high-level overview of your spending by category and provider. Monitor your monthly fluctuations with `get_monthly_trends`, or check if you are staying within your limits using `get_budget_compliance`. You can also identify your most frequent wellness merchants through the `get_provider_loyalty_report` tool.


## Available Tools (4)
- **get_budget_compliance**: Compares actual wellness spending against user-defined budget limits
- **get_monthly_trends**: Analyzes how wellness spending fluctuates over time
- **get_provider_loyalty_report**: You can optionally filter by a minimum spend threshold.

Identifies which providers receive the most frequent or highest volume of wellness spending
- **get_spending_summary**: Provides a high-level overview of total wellness spending across all dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Expense Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my wellness spending from January 1st, 2024 to March 31st, 2024."

**🤖 AI Agent:**
> Your total wellness spend for this period was $450.00. You spent $200.00 on Nutrition, $150.00 on Physical Fitness, and $100.00 on Mental Health. Your top provider was 'Green Smoothies' with $120.00 spent.

---

**👤 You:**
> "Am I within my $200 budget for February 2024?"

**🤖 AI Agent:**
> In February 2024, you spent $185.00. You are $15.00 under your $200.00 budget.

---

**👤 You:**
> "What has my wellness spending trend been like since the start of the year?"

**🤖 AI Agent:**
> Since the start of the year, your wellness spending has been decreasing, moving from $300.00 in January to $250.00 in March.


## ❓ FAQ

**Q: How can I see if I am over my monthly budget?**
You can use the `get_budget_compliance` tool by providing your target monthly budget and the specific month you want to check.

**Q: Can I see which wellness providers I use most often?**
Yes, the `get_provider_loyalty_report` tool identifies your top providers based on total spend and transaction count.

**Q: How do I get a summary of my spending by category?**
Use the `get_spending_summary` tool with a start and end date to receive a breakdown of costs by category, provider, and recurring status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-expense-tracker](https://vinkius.com/en/ai-agent-connect/wellness-expense-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Expense Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-expense-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Expense Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-expense-tracker": {
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

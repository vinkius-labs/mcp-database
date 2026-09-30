# Fundraiser Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fundraiser-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Simulate revenue, expenses, and ticket requirements for fundraising events.

## Description
This MCP server provides financial modeling tools for event organizers. Use `simulate_event_profit` to calculate net profit based on ticket sales, donations, and raffle revenue. Use `calculate_required_tickets` to determine the exact number of attendees needed to reach a specific fundraising target. You can also use `compare_scenarios` to evaluate different budget plans or `analyze_expense_impact` to see how rising vendor costs affect your bottom line.


## Available Tools (4)
- **calculate_required_tickets**: Calculate the number of tickets needed to reach a target net profit
- **analyze_expense_impact**: Analyze how increases in expenses or fees impact the net profit
- **compare_scenarios**: Compare two different fundraising scenarios
- **simulate_event_profit**: Simulate event profit given specific revenue and expense numbers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fundraiser Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I sell 100 tickets at $50 each, get $500 in donations, and have $1000 in vendor costs with a 3% fee, what is my profit?"

**🤖 AI Agent:**
> Your gross revenue is $5,500, your total fees are $165, and your total expenses are $1,000, resulting in a net profit of $4,335.

---

**👤 You:**
> "How many $25 tickets do I need to sell to reach a $2,000 profit if I have $500 in vendor costs and $200 in donations, with a 2.5% fee?"

**🤖 AI Agent:**
> You need to sell 83 tickets to reach your $2,000 profit goal.

---

**👤 You:**
> "What happens to my profit if my vendor costs increase by $200?"

**🤖 AI Agent:**
> An increase of $200 in vendor costs will reduce your net profit by exactly $200.


## ❓ FAQ

**Q: How do I know if my fundraiser will be successful?**
You can use the `simulate_event_profit` tool to input your expected ticket sales, donations, and vendor costs to see your projected net profit.

**Q: How many tickets do I need to sell to reach my goal?**
The `calculate_required_tickets` tool calculates the minimum number of tickets needed to hit your target, accounting for transaction fees.

**Q: Can I compare two different budget plans?**
Yes, use the `compare_scenarios` tool to compare two sets of parameters and see which one yields a higher net profit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fundraiser-budget-planner](https://vinkius.com/en/ai-agent-connect/fundraiser-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fundraiser Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fundraiser-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fundraiser Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fundraiser-budget-planner": {
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

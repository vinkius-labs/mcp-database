# Subscription Killer Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/subscription-killer-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze and optimize recurring expenses to maximize disposable income.

## Description
The Subscription Killer Calculator is a specialized financial intelligence tool designed to help you identify waste in your recurring expenses. By using tools like `calculate_annualized_expenditure`, you can standardize all costs--whether weekly, monthly, or annual--into a single yearly total. The server also provides `analyze_subscription_utility` to pinpoint underutilized services based on your usage frequency, and `model_savings_optimization` to predict exactly how much you could save by cancelling or downgradically changing plans. Additionally, you can use `calculate_freedom_number` to determine the investment capital required to cover all subscriptions through passive income, and `track_trial_deadlines` to ensure you never miss a cancellation window for free trials.


## Available Tools (5)
- **analyze_subscription_utility**: Identify underutilized subscriptions
- **calculate_annualized_expenditure**: Calculate the total annualized cost of all subscriptions
- **calculate_freedom．freedom_number**: Calculate the subscription freedom number
- **model_savings_optimization**: Predict financial gains from subscription changes
- **track_trial_deadlines**: Calculate trial cancellation deadlines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Killer Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have Netflix at $15.99/month and Spotify at $9.99/month. What is my total annual cost?"

**🤖 AI Agent:**
> Your total annualized expenditure is $311.76 per year.

---

**👤 You:**
> "I use Disney+ only 2 times a month. If my threshold is 4 uses, how much can I save if I cancel it? It costs $13.99/month."

**🤖 AI Agent:**
> Cancelling Disney+ would result in an annual savings of $167.88.

---

**👤 You:**
> "How much money do I need invested to cover $2,400 in annual subscriptions if my safe withdrawal rate is 4%?"

**🤖 AI Agent:**
> To cover your $2,400 annual subscription cost with a 4% withdrawal rate, you need a 'freedom number' of $60,000.


## ❓ FAQ

**Q: How does the calculator standardize my costs?**
The `calculate_annualized_expenditure` tool converts all billing cycles (weekly, monthly, and annual) into a standardized yearly total so you can see the true impact of every subscription.

**Q: Can I identify which subscriptions to cancel?**
Yes, by using `analyze_subscription_utility`, you can compare your usage frequency against a threshold to find services that are costing you more than they are worth.

**Q: How do I avoid being charged after a free trial?**
The `track_trial_deadlines` tool calculates the exact date you need to cancel your trial based on a notice buffer period you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/subscription-killer-calculator](https://vinkius.com/mcp/subscription-killer-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Killer Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-killer-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Killer Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-killer-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

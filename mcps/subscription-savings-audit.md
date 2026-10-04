# Subscription Savings Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subscription-savings-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Audit subscription costs, renewal schedules, and usage efficiency.

## Description
This MCP server provides a comprehensive financial audit of your active subscriptions. It allows AI agents to calculate monthly and annual costs, identify upcoming renewal obligations using `get_renewal_calendar`, and pinpoint wasteful spending through `analyze_usage_efficiency`. You can also aggregate spending patterns with `group_subscriptions_by_frequency` or get a high-level overview with `summarize_subscription_costs`.

### Available Tools

`summarize_subscription_costs_tool`, `get_renewal_calendar_tool`, `analyze_usage_efficiency_tool`, `group_subscriptions_by_frequency_tool`


## Available Tools (4)
- **get_renewal_calendar_tool**: Identifies upcoming financial obligations to prevent unexpected charges
- **group_subscriptions_by_frequency_tool**: Breaks down spending patterns based on how often services are billed
- **analyze_usage_efficiency_tool**: Identifies which subscriptions are providing the least value relative to their cost and user count
- **summarize_subscription_costs_tool**: Provides a high-level financial overview of all active subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Savings Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my upcoming subscription renewals for the next 30 days?"

**🤖 AI Agent:**
> You have two upcoming renewals: Netflix on October 15th ($15.99) and Spotify on October 22nd ($9.99).

---

**👤 You:**
> "Show me a summary of my subscription costs."

**🤖 AI Agent:**
> Your total monthly cost is $45.00, and your projected annual total is $540.00. You could save $12.00 by cancelling underutilized services.

---

**👤 You:**
> "Which subscriptions are inefficient if the usage score is below 0.3?"

**🤖 AI Agent:**
> The following subscriptions are inefficient: Disney+ (usage score: 0.1, potential savings: $7.99) and Paramount+ (usage score: 0.2, potential savings: $5.99).


## ❓ FAQ

**Q: How can I see when my next subscription will charge me?**
You can use the `get_renewal_calendar` tool to see all upcoming renewals within a specified number of days. Tools available: `summarize_subscription_costs_tool`, `get_renewal_calendar_tool`, `analyze_usage_efficiency_tool`.

**Q: How do I identify subscriptions that are wasting money?**
Use the `analyze_usage_efficiency` tool with a minimum usage score to find subscriptions that provide low value relative to their cost.

**Q: Can I see my total monthly spending?**
Yes, the `summarize_subscription_costs` tool provides a high-level overview including monthly and annual totals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subscription-savings-audit](https://vinkius.com/en/ai-agent-connect/subscription-savings-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Savings Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-savings-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Savings Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-savings-audit": {
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

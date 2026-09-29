# Subscription Renewal Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subscription-renewal-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze subscription renewals, budget constraints, and usage to generate actionable keep/cancel/review plans.

## Description
This MCP server provides a strategic engine for managing subscription lifecycles. It connects AI agents to your financial data to evaluate renewal schedules against budget limits and usage thresholds. Use `analyze_renewal_schedule` to generate a prioritized calendar of keep, cancel, or review decisions. You can also use `get_owner_action_items` to create to-do lists for subscription owners, `calculate_savings_reallocation` to redistribute funds from cancelled services, and `validate_payment_authorization` to ensure upcoming renewals stay within your budget.


## Available Tools (4)
- **get_owner_action_items**: Generates a specific to-do list for the subscription owners based on the analysis
- **calculate_savings_reallocation**: Determines how much capital is liberated by cancellations and suggests where to move those funds
- **validate_payment_authorization**: Checks if a specific upcoming renewal is financially permissible under current budget constraints
- **analyze_renewal_schedule**: Evaluates all provided subscriptions against notice windows and usage thresholds to generate a prioritized action plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Renewal Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these subscriptions: [{id: '1', name: 'Cloud Storage', owner: 'Alice', price: 50, renewalDate: '2024-12-01', cancellationTerms: 7, usageNotes: 'High usage', usageValue: 100}] with a budget limit of 100 and a usage threshold of 80."

**🤖 AI Agent:**
> The subscription 'Cloud Storage' meets the usage threshold and fits within the budget, so it is marked to Keep.

---

**👤 You:**
> "What actions should the owners take for the current renewal plan?"

**🤖 AI Agent:**
> Alice needs to Cancel 'Streaming Service' by November 25th to avoid the December 1st renewal charge.

---

**👤 You:**
> "How much can I save if I cancel my unused subscriptions?"

**🤖 AI Agent:**
> By cancelling the identified subscriptions, you will liberate $45.00 to be reallocated to your 'Emergency Fund' goal.


## ❓ FAQ

**Q: How does the tool decide to cancel a subscription?**
A subscription is marked for cancellation if its usage value falls below the user-defined threshold or if it causes a breach of the total budget limit.

**Q: Can I redistribute money from cancelled subscriptions?**
Yes, you can use `calculate_savings_reallocation` to suggest how to move funds from cancelled subscriptions into your defined savings goals based on priority.

**Q: What is a notice window?**
The notice window is the timeframe before a renewal occurs during which you must act to cancel the service without being charged for the next period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subscription-renewal-planner](https://vinkius.com/en/ai-agent-connect/subscription-renewal-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Renewal Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-renewal-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Renewal Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-renewal-planner": {
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

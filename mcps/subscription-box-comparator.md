# Subscription Box Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subscription-box-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Evaluate and rank subscription services based on value, flexibility, and item relevance.

## Description
This MCP server provides tools to compare subscription boxes by analyzing financial value, management flexibility, and item relevance. Use `compare_box_value` to find the best deal, `analyze_subscription_flexibility` to check skip policies, `calculate_effective_cost` to normalize pricing across different frequencies, and `evaluate_item_relevance` to predict potential waste based on user preferences.


## Available Tools (4)
- **analyze_subscription_flexibility**: Compares how easy it is to manage or pause subscriptions between two services
- **calculate_effective_cost**: Normalizes different subscription frequencies to a standard monthly cost for fair comparison
- **compare_box_value**: Determines which subscription box offers the best financial value for the user
- **evaluate_item_relevance**: Predicts the waste factor based on the probability of receiving unwanted items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Box Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which box is a better deal: SnackBox or TreatBox?"

**🤖 AI Agent:**
> SnackBox offers the best value with an efficiency ratio of 1.5, compared to TreatBox which has an efficiency ratio of 1.2.

---

**👤 You:**
> "How much will the CoffeeClub cost me per month if it is a quarterly subscription?"

**🤖 AI Agent:**
> The normalized monthly cost for CoffeeClub is $15.00.

---

**👤 You:**
> "Is the BeautyBox flexible enough for someone who wants to skip months?"

**🤖 AI Agent:**
> Yes, BeautyBox allows you to skip deliveries, making it a flexible option.


## ❓ FAQ

**Q: How is the value of a subscription box calculated?**
Value is determined by the efficiency ratio, which is the total estimated market value of the items divided by the total cost (subscription price plus shipping).

**Q: Can I compare monthly and quarterly boxes fairly?**
Yes, you can use the `calculate_effective_cost` tool to normalize different subscription frequencies to a standard monthly cost for a fair comparison.

**Q: What determines the flexibility of a subscription?**
Flexibility is primarily measured by the skip policy. A box that allows you to skip a delivery without canceling is considered more flexible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subscription-box-comparator](https://vinkius.com/en/ai-agent-connect/subscription-box-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Box Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-box-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Box Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-box-comparator": {
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

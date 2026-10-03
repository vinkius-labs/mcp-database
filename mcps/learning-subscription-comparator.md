# Learning Subscription Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/learning-subscription-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare online learning subscriptions by cost, content, and flexibility.

## Description
This MCP server provides tools to analyze online learning platforms. Use `get_subscription_details` to view specific tier information, `compare_value_per_lesson` to find the best cost efficiency, `evaluate_flexibility_risk` to check for lock-in periods, and `calculate_learning_velocity` to compare content consumption speed.


## Available Tools (4)
- **compare_value_per_lesson**: 
- **calculate_learning_velocity**: 
- **evaluate_flexibility_risk**: 
- **get_subscription_details**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Learning Subscription Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which subscription is better value: Coursera Premium or edX Pro?"

**🤖 AI Agent:**
> Coursera Premium offers a better value per lesson at $0.05 per lesson, compared to edX Pro at $0.08 per lesson.

---

**👤 You:**
> "Tell me about the details for the Udemy Business tier."

**🤖 AI Agent:**
> Udemy Business costs $39.99 per month and includes 15,000 lessons with professional certificates included.

---

**👤 You:**
> "Is there a lock-in period for the LinkedIn Learning subscription?"

**🤖 AI Agent:**
> No, the LinkedIn Learning subscription has no mandatory lock-in period and zero cancellation penalty.


## ❓ FAQ

**Q: How can I find the most cost-effective subscription?**
You can use the `compare_value_per_lesson` tool to see the price per individual lesson across different platforms.

**Q: Can I check for cancellation penalties?**
Yes, use `evaluate_flexibility_risk` to determine if a subscription has a lock-in period or high cancellation fees.

**Q: What information is included in the subscription details?**
The `get_subscription_details` tool provides monthly price, total lessons, certificate availability, and estimated hours to complete.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/learning-subscription-comparator](https://vinkius.com/en/ai-agent-connect/learning-subscription-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Learning Subscription Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `learning-subscription-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Learning Subscription Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "learning-subscription-comparator": {
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

# Subscription Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subscription-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate monthly and annual subscription costs and burn rates.

## Description
This MCP server provides tools to calculate the cumulative cost of recurring subscriptions. Use `get_monthly_burn` to find your monthly spending, `get_annual_commitment` for yearly totals, or `get_subscription_summary` for a complete breakdown of both timeframes. You can also use `compare_frequencies` to rank your subscriptions by their annual impact.


## Available Tools (4)
- **get_annual_commitment**: Calculates the total amount a user is committed to spend over a full year
- **get_monthly_burn**: Calculates the total amount a user spends on all subscriptions in a single month
- **get_subscription_summary**: Provides a high-level breakdown of monthly and annual costs in a single request
- **compare_frequencies**: Identifies which subscriptions are the most expensive when viewed on an annual basis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my monthly burn for a $15 Netflix monthly sub and a $120 Amazon annual sub?"

**🤖 AI Agent:**
> Your total monthly burn is $25.

---

**👤 You:**
> "Give me a summary for: Spotify ($10 monthly), Disney+ ($120 annual), and iCloud ($2.99 monthly)."

**🤖 AI Agent:**
> Your monthly total is $22.99, your annual total is $275.88, and you have 3 subscriptions.

---

**👤 You:**
> "Which is more expensive: a $15 monthly gym membership or a $150 annual gym membership?"

**🤖 AI Agent:**
> The $15 monthly gym membership is more expensive, costing $180 annually compared to $150 for the annual membership.


## ❓ FAQ

**Q: How does the monthly burn calculation work?**
The `get_monthly_burn` tool sums all monthly subscription prices and adds the monthly equivalent of annual subscriptions (annual price divided by 12).

**Q: Can I compare different subscription frequencies?**
Yes, you can use `compare_frequencies` to see which subscriptions cost the most on an annual basis, regardless of whether they are billed monthly or annually.

**Q: What information do I need to provide?**
You need to provide a list of subscriptions, each containing a price and a frequency (either 'monthly' or 'annual').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subscription-total-calculator](https://vinkius.com/en/ai-agent-connect/subscription-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-total-calculator": {
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

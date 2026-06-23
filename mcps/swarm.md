# Swarm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swarm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Orchestrate multi-agent AI workflows where specialized agents collaborate, delegate tasks, and solve complex problems together.

## Description
Connect your **Swarm** loyalty account to any AI agent and simplify how you manage customer rewards, award points for transactions, and handle redemptions through natural conversation.

### What you can do

- **Point Management** — Retrieve real-time point balances and loyalty tiers for specific customer IDs.
- **Transaction Processing** — Programmatically award points to customers by registering sale amounts and product data via AI.
- **Reward Redemption** — Convert customer points into discount vouchers or specific rewards and list all active vouchers.
- **Catalog Discovery** — Browse available rewards and check eligibility for specific customers instantly.
- **Voucher Oversight** — List and query all unused discount codes currently assigned to a customer's profile.
- **Loyalty Lifecycle** — Manage the entire customer reward journey directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Swarm API Key (found in your account dashboard)
3. Start managing your loyalty program from your favorite AI assistant

### Who is this for?

- **Retail Business Owners** — quickly check customer points and award rewards during checkout via simple AI commands.
- **Marketing Managers** — monitor reward distribution and verify voucher availability directly from the workspace.
- **Customer Success Teams** — assist customers with point inquiries and handle manual redemptions via the AI assistant.


## Available Tools (5)
- **get_customer_balance**: Check customer loyalty points
- **list_available_rewards**: List redeemable rewards
- **list_customer_vouchers**: List active customer vouchers
- **process_loyalty_transaction**: Process a sale and award points
- **redeem_customer_reward**: Redeem points for a reward


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swarm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the point balance for customer 'cust_10293'?"

**🤖 AI Agent:**
> I've retrieved the balance. Customer cust_10293 currently has 1,250 points and is in the 'Gold Tier'. They are eligible for a 15% discount voucher. Would you like to redeem it now?

---

**👤 You:**
> "Award points for a $150 purchase to customer 'cust_88231'."

**🤖 AI Agent:**
> Transaction processed! I've awarded the points for a $150.00 sale to customer cust_88231. Their new balance is now 1,400 points. The customer has been notified via email.

---

**👤 You:**
> "Show me all available rewards I can claim with 500 points."

**🤖 AI Agent:**
> Fetching reward catalog... With 500 points, you can claim: 'Free Coffee' (200 pts), '10% Discount Code' (400 pts), or 'Sticker Pack' (150 pts). Which one would you like to redeem?


## ❓ FAQ

**Q: Can I check a customer's points balance via AI?**
Yes! Use the `get_customer_balance` tool and provide the Customer ID. Your agent will retrieve the current points and the loyalty tier for that specific user.

**Q: How do I award points for a recent purchase using the agent?**
Use the `process_loyalty_transaction` action. Provide the Customer ID and the transaction amount. The agent will instantly calculate and award the correct points based on your Swarm settings.

**Q: Is it possible to list all the rewards a customer can claim?**
Absolutely. Use the `list_available_rewards` query and provide the Customer ID. The agent will return the catalog of rewards that the user is currently eligible to redeem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swarm](https://vinkius.com/mcp/swarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swarm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swarm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swarm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swarm": {
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

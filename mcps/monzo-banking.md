# Monzo Banking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monzo-banking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Universal Monzo intelligence — check balances, accounts, and transactions via AI.

## Description
Equip your AI agent with real-time personal finance intelligence through the **Monzo** MCP server. This integration provides secure access to your Monzo bank accounts, allowing your agent to retrieve current balances, list multiple accounts, and fetch recent transaction history. Whether you are auditing your personal spending, tracking budget goals, or managing daily finances, your agent acts as a dedicated financial assistant through natural conversation.

### What you can do

- **Balance Inquiry** — Get the real-time balance and daily spending summary for any of your Monzo accounts.
- **Account Listing** — Retrieve a complete list of all bank accounts associated with your profile.
- **Transaction History** — Fetch recent transactions to audit your spending patterns and vendors.
- **Financial Auditing** — Ask your agent to summarize your recent financial activity.

### How it works

1. Subscribe to this server
2. Enter your Monzo Access Token (get it at developers.monzo.com)
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Personal Finance Enthusiasts** — track their spending and balances through simple AI queries.
- **Digital Nomads** — monitor their UK-based Monzo accounts while traveling.
- **Developers** — build automated personal finance workflows and budgeting tools.
- **Busy Professionals** — get quick summaries of their financial status without opening an app.


## Available Tools
- **get_monzo_accounts**: List all Monzo accounts
- **get_monzo_balance**: Get balance for a Monzo account
- **get_monzo_transactions**: Get recent transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monzo Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current Monzo balance."

**🤖 AI Agent:**
> Retrieving your account balance... Your current balance is £1,245.50. You have spent £12.30 so far today. Would you like to see your recent transactions?

---

**👤 You:**
> "List my Monzo accounts."

**🤖 AI Agent:**
> I've found 2 accounts: a 'Personal' account (ending in 4567) and a 'Joint' account (ending in 8901). Which one would you like to check?

---

**👤 You:**
> "What were my last 5 transactions?"

**🤖 AI Agent:**
> Fetching your recent history... Your last 5 transactions include 'Tesco' (£5.40), 'Starbucks' (£3.20), and 'Transport for London' (£2.10). Would you like the full breakdown?


## ❓ FAQ

**Q: Can I see how much I spent today?**
Yes! Use the `get_monzo_balance` tool. The response includes a `spend_today` value that shows your total expenditures for the current day.

**Q: How do I find my Account ID?**
First, call the `get_monzo_accounts` tool. It will return a list of all your accounts with their corresponding GIDs (IDs). Use these IDs for balance and transaction queries.

**Q: Is it safe to share my Monzo token?**
Your token is encrypted at rest and only injected securely at runtime. Never share your token with unauthorized persons. We recommend using a limited-scope token if available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monzo-banking](https://vinkius.com/mcp/monzo-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monzo Banking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `monzo-banking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monzo Banking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monzo-banking": {
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

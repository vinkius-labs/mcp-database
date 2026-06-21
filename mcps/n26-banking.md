# N26 Banking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/n26-banking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Universal N26 intelligence — check balances, accounts, and spaces via AI.

## Description
Equip your AI agent with real-time personal finance intelligence through the **N26** MCP server. This integration provides secure access to your N26 bank accounts, allowing your agent to retrieve current balances, list multiple accounts, and fetch recent transaction history. Your agent can also explore N26 'Spaces' (sub-accounts) to monitor specific savings goals. Whether you are auditing your personal spending, tracking budget goals across Europe, or managing daily finances, your agent acts as a dedicated financial assistant through natural conversation.

### What you can do

- **Balance Inquiry** — Get the real-time balance and IBAN for any of your N26 accounts.
- **Transaction History** — Fetch recent transactions to audit your spending patterns and vendors across the Eurozone.
- **Space Monitoring** — Retrieve details and balances for all your N26 Spaces.
- **Financial Auditing** — Ask your agent to summarize your recent financial activity and sub-account status.

### How it works

1. Subscribe to this server
2. Enter your N26 Access Token (get it at N26 Developer portal)
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Personal Finance Enthusiasts** — track their spending and balances through simple AI queries.
- **European Expats & Digital Nomads** — monitor their N26 accounts while living or traveling across Europe.
- **Sustainable Devs** — build automated personal finance workflows and budgeting tools.
- **Busy Professionals** — get quick summaries of their financial status without opening an app.


## Available Tools
- **get_n26_accounts**: List all N26 accounts
- **get_n26_spaces**: Get N26 spaces and sub-account balances
- **get_n26_transactions**: Get recent N26 transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **N26 Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my N26 account balance."

**🤖 AI Agent:**
> Retrieving your account details... Your current balance is €2,150.40. I've also identified your IBAN if you need it for a transfer. Would you like to see your recent transactions?

---

**👤 You:**
> "What are my last 3 transactions on N26?"

**🤖 AI Agent:**
> Fetching your history... Your last 3 transactions were: 'Lidl' (€15.20), 'Amazon.de' (€45.00), and 'Shell' (€60.00). Would you like to see more details for any of these?

---

**👤 You:**
> "List all my N26 Spaces and their balances."

**🤖 AI Agent:**
> Retrieving your Spaces... You have 3 active spaces: 'Vacation' (€1,200), 'New Car' (€5,000), and 'Emergency Fund' (€2,500). Your total savings across all spaces is €8,700.


## ❓ FAQ

**Q: Can I see my N26 Spaces balance?**
Yes! Use the `get_n26_spaces` tool. It will return a list of all your sub-accounts (Spaces) along with their specific current balances.

**Q: Does this support transactions from all merchants?**
The `get_n26_transactions` tool retrieves all visible transactions in your history, providing the merchant name or partner name as recorded by N26.

**Q: Is my banking data secure?**
Yes. Your access token is encrypted at rest and only injected securely at runtime. The MCP server acts as a secure proxy and does not store your login credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/n26-banking](https://vinkius.com/mcp/n26-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **N26 Banking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `n26-banking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **N26 Banking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "n26-banking": {
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

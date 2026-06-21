# Fintoc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fintoc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Access bank accounts, movements, and initiate transfers via AI agents with Fintoc.

## Description
Connect your **Fintoc** account to any AI agent and automate your open banking and payment operations through the Model Context Protocol (MCP). Fintoc is the leading API for financial integration in Latin America (Chile and Mexico), allowing you to securely access real-time bank data and programmatically initiate transfers.

### What you can do

- **Bank Connectivity** — List and manage your active bank links to maintain persistent access to financial data.
- **Account Inspections** — Fetch detailed information for all linked bank accounts, including available balances and holder details.
- **Movement History** — Retrieve transaction history (movements) for any account with powerful filtering options by date.
- **Payment Initiation** — Create and monitor payment intents to automate bank transfers directly through the agent.
- **Subscription Tracking** — List and manage active subscriptions to keep track of recurring payments.
- **Institution Discovery** — Discover supported banks and financial institutions across different countries (Chile and Mexico).
- **Real-time Monitoring** — Fetch specific movement details or payment intent statuses to keep your financial operations in sync.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fintoc Secret Key (found in your Fintoc Dashboard)
3. Start managing your open banking data and transfers from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Teams** — automate the gathering of bank movements for reconciliation and audit reports.
- **Fintech Developers** — quickly test and integrate open banking flows without leaving your development environment.
- **Business Owners** — get a unified view of your bank balances and transaction history through simple AI commands.


## Available Tools
- **create_payment_intent**: Create a payment intent
- **get_account**: Get account details
- **get_link**: Get link details
- **get_movement**: Get movement details
- **get_payment_intent**: Get payment intent details
- **get_subscription**: Get subscription details
- **list_accounts**: List accounts for a link
- **list_institutions**: List supported institutions
- **list_links**: List all links
- **list_movements**: List movements for an account
- **list_payment_intents**: List payment intents
- **list_subscriptions**: List subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fintoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bank accounts linked to Fintoc."

**🤖 AI Agent:**
> Fetching accounts... I found 2 accounts linked to your Fintoc profile: 'Checking Account (...1234)' with a balance of 500,000 CLP and 'Savings Account (...5678)' with 1,200,000 CLP.

---

**👤 You:**
> "Show me the last 5 transactions for account 'acc_9876'."

**🤖 AI Agent:**
> Retrieving movements... Here are the 5 most recent transactions for account acc_9876, including 'Starbucks' (-4,500 CLP) and 'Amazon Prime' (-12,000 CLP).

---

**👤 You:**
> "Which banks are supported in Chile (cl)?"

**🤖 AI Agent:**
> Checking institutions... In Chile, Fintoc supports major banks including Banco de Chile, Banco Santander, Banco Estado, BCI, and Scotiabank. Would you like the full list?


## ❓ FAQ

**Q: Which countries are supported by the Fintoc MCP server?**
Fintoc currently supports major financial institutions in Chile (cl) and Mexico (mx). You can use the 'list_institutions' tool to see the specific banks available in each region.

**Q: Can I filter bank movements by specific dates using the agent?**
Yes! The 'list_movements' tool accepts 'since' and 'until' parameters in ISO format. For example, you can ask the agent to 'List movements from 2023-01-01 to 2023-01-31' for a specific account.

**Q: How secure is my bank data when using Fintoc through Vinkius?**
Your security is paramount. Vinkius encrypts your Fintoc Secret Key at rest and only injects it into the isolated execution environment. Fintoc uses read-only access for movements and bank-grade security for all operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fintoc](https://vinkius.com/mcp/fintoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fintoc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fintoc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fintoc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fintoc": {
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

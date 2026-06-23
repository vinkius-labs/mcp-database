# Treinta App MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/treinta-app)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Empower Latin American SMBs automating Treinta app. Access ledgers, manage client debt, and review store inventories actively from chat.

## Description
Connect your **Treinta SMB** store operator account directly to Vurb allowing Claude to perform deep digital bookkeeping natively.

### What you can do

- **Write Real Transactions** — Easily ask to compute ''I sold two coffees for $10'' and watch it register into your daily accounting books seamlessly.
- **Check Client Tab (Fiado)** — Access the registered client list and rapidly probe who currently has an unpaid debt.
- **Audit Inventory** — Download your digital stock catalog reading precise shelf margins instantly.
- **Macro Profit & Loss** — Pull your dashboard KPIs asserting if your monthly operational balances ended green.

### How it works

1. Append the node 
2. Integrate the official bearer Dev Token exported privately by Treinta.
3. Instruct your Agent to behave like your most proactive virtual business manager.

### Who is this for?

- **Micro Business Owners** — Not wanting to open the mobile App while checking computer figures on Sunday nights.
- **Retail Accountants** — Reading multiple stores margins continuously.
- **SMB Tech Enthusiasts** — Bridging Latin American retail solutions with localized GPT autonomous prompts.


## Available Tools (12)
- **create_client**: Register a new active client
- **create_product**: Add a new store inventory product
- **create_transaction**: Create a new business transaction
- **delete_transaction**: Revert an incorrect transaction
- **get_business_stats**: Get macro P&L operations dashboard
- **get_client**: Fetch specific client debt profile
- **get_product**: Fetch targeted product SKU details
- **list_clients**: List registered customers/clients
- **list_products**: Get complete business inventory
- **list_sales**: List consolidated sales
- **list_transactions**: List book flow transactions
- **update_product_stock**: Update physical quantity of a product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Treinta App** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit the store today. Check recent logged transactions and summarize our business overall dashboard stats."

**🤖 AI Agent:**
> Running deep audit natively! From recent logs, we observed a steady 'Expense' tied to utilities and 3 minor 'Income' retail transactions. Pulling P&L Dashboard confirms an aggregated positive Net Margin resting globally at 2.5K. Cashflow looks healthy.

---

**👤 You:**
> "Create a formal Income Transaction representing our $35 cash sale of the surplus store products."

**🤖 AI Agent:**
> Transaction pushed successfully onto ledgers! Stamped '$35' under 'Income' tagging surplus. Refreshed data rests native on your mobile app instantly.

---

**👤 You:**
> "Delete this transaction id 123"

**🤖 AI Agent:**
> Done.


## ❓ FAQ

**Q: Can I effectively add a transaction manually into my Treinta log via chat?**
Absolutely. Target the `create_transaction` pipeline expressing clearly if it is 'income' or 'expense' plus the numeral amount, and the AI correctly syncs your local digital accountant book over to proper state.

**Q: Is the Treinta token key shielded visually so employees cannot read it out?**
Yes. Following protocol standard, all credentials marked within the SMB Accounting group carry underlying `sensitive: true` parameters natively wiping the true key from console displays.

**Q: Are operations retroactive?**
Yes, if you fetch the right dates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/treinta-app](https://vinkius.com/mcp/treinta-app)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Treinta App** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `treinta-app` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Treinta App** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "treinta-app": {
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

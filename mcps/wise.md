# Wise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to Wise — check multi-currency balances, track international transfers, and manage recipients without opening the banking interface.

## Description
Connect your **Wise** Business account to your AI agent and manage international payments and multi-currency operations conversationally.

### What you can do

- **Multi-Currency Balances** — Check real-time balances across all your currency accounts (USD, EUR, GBP, and 50+ currencies) instantly.
- **Transfer Tracking** — Monitor the status of outgoing transfers, view estimated delivery dates, and check exchange rates applied.
- **Recipient Management** — List, search, and manage your payment recipients across countries and currencies.
- **Exchange Rates** — Get live exchange rates and compare costs before initiating transfers.

### How it works

1. Subscribe to the Wise integration on the marketplace.
2. Generate a Personal API Token from your Wise Business account (Settings → API tokens → Add new token).
3. Ask your AI agent to check balances, track transfers, or manage recipients.

### Who is this for?

- **International Businesses** — Monitor multi-currency cash positions across global operations without logging into the Wise dashboard.
- **Finance Teams** — Track FX rates and transfer statuses for month-end reconciliation and treasury management.
- **Freelancers & Agencies** — Check incoming payments from international clients and manage multi-currency invoicing from your AI assistant.


## Available Tools
- **list_profiles**: List Wise business profiles
- **get_currencies**: List supported currencies
- **list_balances**: List multi-currency balances
- **get_balance**: Get specific balance details
- **list_recipients**: List payment recipients
- **create_quote**: Create a transfer quote
- **list_transfers**: List all transfers
- **get_transfer**: Get transfer details
- **get_exchange_rate**: Get live exchange rate
- **list_statements**: List account statements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my current balances across all currencies?"

**🤖 AI Agent:**
> Here are your Wise balances: USD $85,200.00, EUR €42,100.00, GBP £18,500.00, and BRL R$15,800.00. Total equivalent: approximately $167,400 USD.

---

**👤 You:**
> "Get me a quote to send €10,000 from my EUR balance to a USD account."

**🤖 AI Agent:**
> Quote ready: €10,000 → $10,842.50 USD at a rate of 1.0850. Wise fee: €28.50. Estimated delivery: 1 business day. The recipient will receive $10,842.50.

---

**👤 You:**
> "Track the status of my recent transfer to our London office."

**🤖 AI Agent:**
> Your transfer of £15,000 to 'London Office Ltd' is currently in 'Processing' stage. Exchange rate locked at 1.2650 (USD→GBP). Estimated delivery: tomorrow by 3:00 PM GMT.


## ❓ FAQ

**Q: How do I get my Wise API token?**
You need a **Wise Business account** with 2-Step Verification enabled. Log in at **wise.com**, click your profile icon in the top right corner, then go to **Settings → API tokens → Add new token**. Name your token, complete the 2-Step Verification, and copy it immediately — it is only shown once. Paste it into the configuration below. Note: this feature is only available on the web — not the mobile app.

**Q: Can I check how much a transfer will cost before sending money?**
Yes. Ask your AI agent to get a quote for any currency pair and amount. It returns the live exchange rate, Wise's fee, the estimated delivery time, and the exact amount the recipient will receive — so you can make informed decisions before committing to a transfer.

**Q: What if I need to track a transfer that seems delayed?**
Just ask your AI agent 'What's the status of my last transfer?' It returns the current processing stage, estimated delivery date, exchange rate used, and any holds or compliance reviews in progress — all without opening Wise in a browser or switching contexts.

**Q: Is this suitable for companies operating in multiple currencies?**
Absolutely. Wise supports 50+ currencies, and your AI agent can check balances in all of them simultaneously. Perfect for global e-commerce businesses, international agencies, remote-first companies paying contractors worldwide, and treasury teams managing FX exposure across multiple regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wise](https://vinkius.com/mcp/wise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wise": {
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

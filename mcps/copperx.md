# Copperx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copperx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Equip your AI agent to manage crypto payments, invoices, and subscriptions directly with Copperx.

## Description
Integrate **Copperx**, the API-first crypto payment processor, directly into your AI workflow. Automate your web3 billing, manage customer subscriptions, and track payouts using natural language.

### What you can do

- **Payment Links** — Create and manage checkout links for products or services instantly.
- **Subscription Management** — List and monitor active recurring billing cycles.
- **Invoicing** — Generate and track crypto invoices for your global customers.
- **Wallet Insights** — Check your account balances across multiple chains and currencies.

### How it works

1. Connect the Copperx integration to your AI assistant.
2. Authorize using your Copperx API Key (found in your dashboard Settings).
3. Manage your crypto treasury and payments through chat.

### Who is this for?

- **Web3 Startups** — Streamline customer onboarding and recurring revenue tracking.
- **Freelancers & DAOs** — Quickly generate payment links or check payout statuses.
- **E-commerce Platforms** — Monitor real-time payment intents and crypto balances.


## Available Tools (10)
- **create_customer**: Creates a new customer record with identity properties (email, name) for future payment associations.

Register a new customer in Copperx
- **create_payment_link**: Resolves product identity and pricing configuration to generate a unique payment URL.

Create a new payment link for customers to pay
- **get_wallet_balance**: Resolves real-time wallet balances across various supported cryptocurrencies and networks.

Check current crypto wallet balances in Copperx
- **get_payment_details**: Resolves granular transaction data, including blockchain tx hashes, fee breakdowns, and customer linkages.

Get details for a specific payment intent
- **list_customers**: Resolves customer identity properties such as unique identifiers, email addresses, and registered names.

List all customers registered in Copperx
- **list_invoices**: Resolves billing document properties including invoice numbers, totals, and payment status links.

List all invoices generated
- **list_payment_links**: Resolves link metadata including checkout URLs, pricing data, and usage statistics.

List all payment links created
- **list_payments**: Resolves payment identity properties including transaction IDs, amounts, currencies, and processing status across the crypto-payment boundary.

List all payment intents in Copperx
- **list_payouts**: Resolves disbursement data including payout IDs, destination wallet addresses, and settlement status.

List all payouts processed
- **list_subscriptions**: Resolves subscription properties including plan IDs, billing cycles, and current subscription state.

List all active and past subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copperx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a crypto payment link for 'Consulting Service' worth 100 USDC."

**🤖 AI Agent:**
> I've created your payment link for 'Consulting Service'. Customers can pay 100 USDC using this URL: [Link]. Would you like me to email this to a customer?

---

**👤 You:**
> "Check my current account balances across all crypto wallets."

**🤖 AI Agent:**
> Your total balance is equivalent to $12,450. Breakdown: 10,000 USDC (Polygon), 1.2 ETH (Mainnet), and 500 MATIC. Would you like to see the recent transaction history?

---

**👤 You:**
> "List all active subscriptions and their monthly revenue."

**🤖 AI Agent:**
> You have 45 active subscriptions generating approximately 4,500 USDC per month. 5 new subscribers joined this week. Should I pull a detailed report?


## ❓ FAQ

**Q: How do I get a Copperx API Key?**
Log in to your Copperx dashboard, navigate to **Settings > API Keys**, and generate a new key. You can use either Test or Live keys depending on your needs.

**Q: Which cryptocurrencies are supported?**
Copperx supports major assets like USDC, USDT, ETH, and MATIC across multiple chains including Ethereum, Polygon, and Solana.

**Q: Can I create recurring subscriptions via chat?**
Yes, you can instruct the agent to create payment links or customers that can be tied to subscription plans defined in your Copperx account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copperx](https://vinkius.com/mcp/copperx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copperx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `copperx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copperx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copperx": {
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

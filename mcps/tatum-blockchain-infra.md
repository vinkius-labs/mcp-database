# Tatum (Blockchain Infra) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tatum-blockchain-infra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Simplify blockchain development with Tatum — estimate fees, track portfolios, and manage real-time webhook subscriptions across multiple chains.

## Description
Connect your **Tatum** account to any AI agent to streamline blockchain infrastructure management. Access real-time data, gas estimates, and portfolio tracking across 40+ protocols through natural language.

### What you can do

- **Fee Estimation** — Get recommended fees or estimate gas for EVM transactions to optimize costs using `get_recommended_fee` and `estimate_evm_gas`.
- **Portfolio Tracking** — Retrieve balances for native assets, ERC-20 tokens, and NFTs across multiple addresses with `get_wallet_portfolio`.
- **Real-time Monitoring** — Create and manage webhook subscriptions for incoming/outgoing transactions using `create_subscription` and `list_subscriptions`.
- **Transaction History** — Query detailed historical data for specific blockchain addresses via `get_transaction_history`.
- **Exchange Rates** — Get live exchange rates between crypto and fiat currencies using `get_exchange_rate`.

### How it works

1. Subscribe to this server
2. Enter your Tatum API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Quickly estimate gas and debug transactions without leaving the IDE
- **DeFi Analysts** — Monitor portfolios and exchange rates in real-time through conversation
- **Ops Teams** — Automate webhook management for blockchain event monitoring


## Available Tools
- **cancel_subscription**: Cancel a webhook subscription
- **create_subscription**: ).

Create a webhook subscription
- **create_virtual_account**: Create a virtual account (off-chain ledger)
- **estimate_evm_gas**: Estimate EVM gas limit and price
- **estimate_transaction_fee**: ).

Estimate transaction fee
- **get_exchange_rate**: Get exchange rate for a crypto or fiat asset
- **get_recommended_fee**: Get recommended fee for a blockchain
- **get_transaction_history**: Get transaction history for an address
- **get_virtual_account_balance**: Get virtual account balance
- **get_wallet_portfolio**: Get wallet portfolio balances
- **list_subscriptions**: List active webhook subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tatum (Blockchain Infra)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the recommended fees for a transaction on Ethereum right now?"

**🤖 AI Agent:**
> I've retrieved the current fee suggestions for ETH: Fast: 25 Gwei, Standard: 20 Gwei, Slow: 15 Gwei. Would you like to estimate the total cost for a specific transfer amount?

---

**👤 You:**
> "Show me the portfolio for address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e on Polygon."

**🤖 AI Agent:**
> Checking the Polygon network... This address holds 15.5 MATIC, 250 USDC (ERC-20), and 2 NFTs from the 'Polygon Punks' collection. Do you need the transaction history for these assets?

---

**👤 You:**
> "What is the current exchange rate from BTC to USD?"

**🤖 AI Agent:**
> The current exchange rate is 1 BTC = 64,250.50 USD. Would you like to check the rate for another pair or calculate a specific conversion?


## ❓ FAQ

**Q: Can I estimate gas for a specific EVM transaction before sending it?**
Yes! Use the `estimate_evm_gas` tool by providing the chain, sender, recipient, and amount. It will return the estimated gas limit and price for that specific interaction.

**Q: How do I monitor a wallet for new incoming transactions automatically?**
You can use the `create_subscription` tool to set up a webhook. This allows you to receive real-time notifications whenever a transaction occurs on the specified address and chain.

**Q: Can I check balances for multiple token types at once?**
Yes, the `get_wallet_portfolio` tool allows you to specify token types like 'native', 'fungible' (ERC-20), and 'nft' to get a comprehensive view of an address's holdings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tatum-blockchain-infra](https://vinkius.com/mcp/tatum-blockchain-infra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tatum (Blockchain Infra)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tatum-blockchain-infra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tatum (Blockchain Infra)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tatum-blockchain-infra": {
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

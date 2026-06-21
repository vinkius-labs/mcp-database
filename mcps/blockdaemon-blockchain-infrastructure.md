# Blockdaemon (Blockchain Infrastructure) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockdaemon-blockchain-infrastructure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access institutional-grade blockchain data across multiple protocols — list blocks, track transactions, and retrieve financial reports via Blockdaemon Ubiquity.

## Description
Connect your **Blockdaemon** account to any AI agent to interact with major blockchain protocols through a single, unified interface. This MCP server leverages the Ubiquity API to provide seamless access to multi-chain data.

### What you can do

- **Block Exploration** — Retrieve block identifiers and metadata for protocols like Bitcoin, Ethereum, Solana, and Polkadot using `list_blocks`.
- **Transaction Tracking** — Query full transaction histories for specific account addresses across supported networks with `list_transactions`.
- **UTXO Management** — Fetch Unspent Transaction Outputs for UTXO-based chains (Bitcoin, Dogecoin, Litecoin) using `get_utxos`.
- **Financial Reporting** — Generate detailed financial reports for addresses on protocols like Algorand, Stellar, and Tezos via `get_financial_report`.
- **Multi-Network Support** — Switch between mainnet and testnet environments effortlessly for development and auditing.

### How it works

1. Subscribe to this server
2. Enter your Blockdaemon API Key
3. Start querying blockchain data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Debug transactions and verify block data without leaving your IDE.
- **Data Analysts** — Aggregate financial reports and transaction histories for cross-chain auditing.
- **Crypto Operations** — Monitor wallet activity and UTXO sets for treasury management.


## Available Tools
- **list_blocks**: Get a list of block identifiers
- **get_financial_report**: Get a financial report for an address
- **list_transactions**: Get a list of transactions for an address
- **get_utxos**: Get Unspent Transaction Outputs (UTXOs)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blockdaemon (Blockchain Infrastructure)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blocks on Ethereum mainnet."

**🤖 AI Agent:**
> I've retrieved the latest blocks for Ethereum mainnet using `list_blocks`. The most recent block height is 19283746 with hash 0xabc...123. Would you like to see the transactions inside this block?

---

**👤 You:**
> "Show me the transaction history for Bitcoin address 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa."

**🤖 AI Agent:**
> Fetching transactions via `list_transactions`... I found 15 recent transactions for this address. The latest was a transfer of 0.5 BTC on 2023-10-25. Should I provide the details for the last 5?

---

**👤 You:**
> "Get a financial report for Algorand address [ADDRESS] on mainnet."

**🤖 AI Agent:**
> Generating the report using `get_financial_report`... The report for the Algorand address is ready. It includes total balance, rewards earned, and transaction volume for the specified period.


## ❓ FAQ

**Q: Which protocols are supported for financial reports?**
The `get_financial_report` tool currently supports Algorand, Polkadot, Stellar, Tezos, and XRP.

**Q: Can I filter transactions by date?**
Yes, the `list_transactions` tool allows you to provide 'from' and 'to' Unix timestamps to narrow down your search.

**Q: How do I check unspent balances for Bitcoin?**
Use the `get_utxos` tool with the 'bitcoin' protocol and the specific wallet address. You can also toggle 'check_mempool' to include unconfirmed transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockdaemon-blockchain-infrastructure](https://vinkius.com/mcp/blockdaemon-blockchain-infrastructure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blockdaemon (Blockchain Infrastructure)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blockdaemon-blockchain-infrastructure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blockdaemon (Blockchain Infrastructure)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blockdaemon-blockchain-infrastructure": {
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

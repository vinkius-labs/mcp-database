# Covalent MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/covalent)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Equip your AI agent to query unified blockchain data including balances, transactions, and NFTs across 100+ chains.

## Description
Integrate **Covalent**, the unified API for blockchain data, directly into your AI workflow. Access real-time and historical data across Ethereum, Polygon, Binance Smart Chain, and over 100 other supported networks using natural language.

### What you can do

- **Wallet Insights** — Retrieve token balances, historical portfolio values, and transaction history for any wallet address.
- **NFT Discovery** — List NFT balances and metadata across supported chains.
- **Transaction Auditing** — Get full details and log events for specific transaction hashes.
- **Network Monitoring** — Check block details and monitor supported chain statuses.

### How it works

1. Connect the Covalent integration to your AI assistant.
2. Authorize using your Covalent API Key (found in your dashboard at covalenthq.com).
3. Query global blockchain data through intuitive conversation.

### Who is this for?

- **Web3 Developers** — Quickly audit smart contract interactions and verify transaction logs.
- **Crypto Investors** — Track portfolio performance and monitor wallet activities across multiple chains.
- **Data Analysts** — Retrieve structured on-chain data for research and reporting via chat.


## Available Tools
- **get_token_balances**: Resolves contract addresses, ticker symbols, token decimals, and current balances (formatted and raw) for the specified wallet and chain.

Get token balances for a wallet address on a specific chain
- **get_block_details**: Resolves block hashes, parent hashes, timestamps, and transaction counts for the specified chain.

Get details for a specific block height
- **get_chains_status**: Resolves block height lag, current sync status, and API availability across all supported networks.

Get the current indexing status of all supported chains
- **get_dex_pools**: Resolves liquidity pool addresses, token pairs, reserve amounts, and volume metrics for the specified DEX.

List liquidity pools for a DEX on a specific chain
- **get_nft_balances**: Resolves NFT contract names, token IDs, metadata URLs, and image links across the specified blockchain network.

Get NFT balances for a wallet address
- **get_historical_portfolio**: Resolves daily balances, asset valuations in USD, and historical price points for the specified wallet.

Get historical daily portfolio value for a wallet address
- **get_token_transfers**: Resolves sender/receiver addresses, transfer values, and transaction timestamps for the specified wallet.

Get historical token transfers for a wallet address
- **get_transaction_details**: Touches raw log events, decoded event parameters, and gas consumption metrics boundary.

Get full details and logs for a specific transaction hash
- **get_transactions**: Resolves transaction hashes, block heights, timestamps, and log events for the specified wallet on the given chain.

Get transaction history for a wallet address
- **list_supported_chains**: Resolves chain IDs, human-readable names, and supported features (NFTs, Dex, etc.) for each blockchain.

List all blockchains supported by Covalent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Covalent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the token balances for address '0x123...' on eth-mainnet."

**🤖 AI Agent:**
> I found 5 tokens for that address. Total value is approximately $1,250. Breakdown: 0.5 ETH, 500 USDC, and 1,200 MATIC. Would you like to see the historical portfolio value?

---

**👤 You:**
> "List the last 10 transactions for address '0x123...' on matic-mainnet."

**🤖 AI Agent:**
> I've retrieved the last 10 transactions. Most involve interactions with Uniswap and Aave. 2 transactions failed due to out-of-gas errors. Should I provide details for a specific transaction?

---

**👤 You:**
> "What are the NFT holdings for wallet '0x123...' on eth-mainnet?"

**🤖 AI Agent:**
> This wallet holds 3 NFTs: 1 Bored Ape Yacht Club, 1 CryptoPunks, and 1 Art Blocks piece. Would you like to see the metadata or the last sale price for any of these?


## ❓ FAQ

**Q: How do I get a Covalent API Key?**
Log in to your Covalent dashboard at covalenthq.com and generate an API Key. You can use the free tier to get started.

**Q: Which blockchains are supported?**
Covalent supports over 100 chains including Ethereum, Polygon, BSC, Avalanche, Fantom, and many Layer 2 solutions like Arbitrum and Optimism.

**Q: Can the agent send transactions?**
No, this integration is for querying data only. It provides high-granularity visibility into on-chain activities but cannot execute writes or sign transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/covalent](https://vinkius.com/mcp/covalent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Covalent** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `covalent` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Covalent** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "covalent": {
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

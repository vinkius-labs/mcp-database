# DeBank (DeFi Wallet Tracker) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/debank-defi-wallet-tracker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/debank-defi-wallet-tracker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/debank-defi-wallet-tracker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track DeFi portfolios, analyze protocols, and monitor wallet history across multiple chains using DeBank's comprehensive data.

## Description
Connect your **DeBank** account to any AI agent and gain deep insights into the DeFi ecosystem. Monitor wallet balances, analyze protocol positions, and track token movements across all supported chains through natural conversation.

### What you can do

- **Portfolio Tracking** — Get total balances, token lists, and used chains for any wallet address.
- **Protocol Analysis** — Inspect specific DeFi protocols, list all protocols on a chain, and analyze complex protocol positions.
- **Token Insights** — Fetch token details, historical prices, and identify top holders for any asset.
- **Transaction Tools** — Explain transactions, pre-execute transfers to estimate outcomes, and monitor gas markets.
- **Security Auditing** — List token and NFT authorizations to manage wallet permissions and exposure.

### How it works

1. Subscribe to this server
2. Enter your DeBank Cloud Access Key
3. Start querying on-chain data from Claude, Cursor, or any MCP-compatible client

No more manually checking multiple block explorers or DeFi dashboards. Your AI acts as a personal crypto analyst and portfolio manager.

### Who is this for?

- **DeFi Traders** — quickly check positions and balances across dozens of protocols without leaving your workflow.
- **Web3 Developers** — analyze token contracts, gas prices, and transaction logic directly from your IDE.
- **Crypto Researchers** — aggregate data on protocol growth, token distribution, and historical pricing via simple prompts.


## Available Tools
- **explain_tx**: Explain Tx
- **get_account_units**: Get API account units usage
- **get_chain**: Get chain information
- **get_gas_market**: Get gas prices
- **get_pool**: Get pool information
- **get_protocol**: Get protocol information
- **get_token_history_price**: Get token history price
- **get_token**: Get token information
- **get_token_top_holders**: Get top holders of token
- **get_user_all_complex_protocol_list**: Get user complex protocol list (all chains)
- **get_user_complex_protocol_list**: Get user complex protocol list (single chain)
- **get_user_history_list**: Get user history list
- **get_user_nft_authorized_list**: Get user authorized NFT list
- **get_user_protocol_positions**: Get user protocol positions
- **get_user_token_authorized_list**: Get user authorized token list
- **get_user_token_list**: Get user token list
- **get_user_total_balance**: Get user total balance
- **get_user_used_chain_list**: Get user used chain list
- **list_all_protocols**: Get all protocols of supported chains
- **list_app_protocols**: Get list of app-protocol information
- **list_chains**: Get supported chain list
- **list_protocols**: Get list of protocol information
- **list_tokens_by_ids**: Get list of token information
- **pre_exec_tx**: Enhanced transaction pre-execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeBank (DeFi Wallet Tracker)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the total balance and the list of chains used by wallet 0x123..."

**🤖 AI Agent:**
> I've analyzed the wallet. The total balance is $45,230.50. This user is active on 4 chains: Ethereum, BSC, Polygon, and Arbitrum. Would you like to see the specific token breakdown for any of these?

---

**👤 You:**
> "Who are the top holders for the token 0x... on Ethereum?"

**🤖 AI Agent:**
> Fetching top holders... The largest holder (excluding contracts) owns 12.5% of the supply. There are currently 3 wallets holding more than 5% of the total circulating supply. Should I list the top 10 addresses?

---

**👤 You:**
> "List all DeFi protocols supported on the Polygon chain."

**🤖 AI Agent:**
> I've retrieved the list for Polygon. There are over 50 supported protocols, including Aave V3, QuickSwap, and Curve. Are you looking for a specific type of protocol, like DEXs or Lending platforms?


## Installation & Usage

To install and use the **DeBank (DeFi Wallet Tracker)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/debank-defi-wallet-tracker](https://vinkius.com/mcp/debank-defi-wallet-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

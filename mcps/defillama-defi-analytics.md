# DefiLlama (DeFi Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/defillama-defi-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/defillama-defi-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/defillama-defi-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access comprehensive DeFi data including TVL, token prices, yields, and volumes across multiple chains and protocols.

## Description
Connect your AI agent to **DefiLlama**, the leading aggregator for decentralized finance data. This server allows you to query real-time and historical metrics across the entire DeFi ecosystem through natural conversation.

### What you can do

- **TVL Analytics** — Track Total Value Locked (TVL) for specific protocols, individual chains, or the global DeFi market.
- **Token Pricing** — Retrieve current and historical prices, generate price charts, and calculate percentage changes for thousands of tokens.
- **Yield & Pools** — Monitor APY and TVL for liquidity pools to identify the best yield farming opportunities.
- **Volume & Liquidity** — Analyze DEX volumes, bridge activity, and stablecoin market caps across different ecosystems.
- **Historical Deep-Dives** — Access time-series data to understand market trends and protocol growth over time.

### How it works

1. Subscribe to this server
2. (Optional) Enter your DefiLlama API Key if you have a pro account, or leave blank for public access
3. Start analyzing the DeFi markets directly from your AI client

### Who is this for?

- **Crypto Analysts** — perform deep on-chain research and protocol comparisons without manual data scraping
- **DeFi Developers** — integrate real-time price and TVL data into your development workflow
- **Portfolio Managers** — track market trends and yield opportunities across multiple chains instantly


## Available Tools
- **get_all_bridges**: Get all bridges
- **get_all_chains_tvl**: Get current TVL for all chains
- **get_all_pools**: Get current APY and TVL for all pools
- **get_all_stablecoins**: Get all stablecoins
- **get_bridge_volume_chain**: Get bridge volume for a specific chain
- **get_current_prices**: Format: {chain}:{address}

Get the current price of tokens
- **get_current_tvl_chain**: Get the current total TVL for a specific chain
- **get_dex_volume_chain**: Get DEX volume for a specific chain
- **get_dex_volumes_global**: Get DEX volumes globally
- **get_historical_prices**: Get the price of tokens at a specific timestamp
- **get_historical_tvl_chain**: Get historical TVL for a specific blockchain
- **get_historical_tvl_global**: Get historical TVL of the entire DeFi ecosystem
- **get_percentage_change**: Get the price change over a period
- **get_pool_historical_data**: Get historical APY and TVL for a specific pool
- **get_price_chart**: Get a chart of token prices over time
- **get_protocol**: Get historical TVL data for a specific protocol
- **get_protocols**: Get all protocols on DefiLlama along with their current TVL
- **get_stablecoin_historical_data**: Get stablecoin historical data
- **get_stablecoin_market_cap_chain**: Get stablecoin market cap for a specific chain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DefiLlama (DeFi Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all DeFi protocols and their current TVL."

**🤖 AI Agent:**
> I've retrieved the list of protocols. Currently, Lido leads with a TVL of $28.4B, followed by EigenLayer and Aave. Would you like to see the historical data for any of these?

---

**👤 You:**
> "What is the current TVL on the Arbitrum chain?"

**🤖 AI Agent:**
> The current Total Value Locked on Arbitrum is approximately $2.56 billion. This represents the aggregate value across all supported protocols on that network.

---

**👤 You:**
> "Show me the price chart for USDC on Ethereum."

**🤖 AI Agent:**
> Fetching the price chart for USDC (ethereum:0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48)... The data shows a stable peg at $1.00 with minor fluctuations over the last 24 hours.


## Installation & Usage

To install and use the **DefiLlama (DeFi Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/defillama-defi-analytics](https://vinkius.com/mcp/defillama-defi-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

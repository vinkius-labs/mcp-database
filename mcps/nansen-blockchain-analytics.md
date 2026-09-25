# Nansen (Blockchain Analytics) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nansen-blockchain-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access institutional-grade blockchain analytics — track Smart Money, profile wallets, and monitor real-time token flows across multiple chains.

## Description
Connect your **Nansen** API to any AI agent to unlock deep on-chain insights through natural language. Nansen provides the data that helps investors and teams identify opportunities and perform due diligence on-chain.

### Key Capabilities

- **Smart Money Tracking** — Monitor where the most sophisticated on-chain entities are moving their capital with netflow and holdings tools.
- **Wallet Profiling** — Inspect any address or entity to see current balances, historical snapshots, and behavioral labels.
- **PnL Analysis** — Calculate aggregate profit and loss for specific wallets or deep dive into performance for individual tokens.
- **DEX & Perp Activity** — Track real-time trading on decentralized exchanges and perpetual platforms like Hyperliquid.
- **Entity Search** — Quickly find tokens, entities, or contract addresses by name or symbol.

### How it works

1. Subscribe to this server
2. Enter your Nansen API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Researchers** — identify emerging trends and whale movements without manual dashboard navigation.
- **Traders** — monitor Smart Money flows and PnL metrics directly from their workspace.
- **Developers** — integrate on-chain labels and balance data into their development workflow.


## Available Tools (48)
- **agent_expert**: Provide the detailed prompt in the body.

Deep multi-step analysis and synthesis
- **agent_fast**: Provide the query details in the body.

Low-latency streamed answers for simple research questions
- **perp_leaderboard**: Pass the required body payload.

Most profitable Hyperliquid traders
- **points_address**: Provide the wallet address as the required input.

Tier lookup for a wallet on the Nansen points leaderboard
- **points_leaderboard**: Paginated Nansen points leaderboard
- **portfolio_defi_holdings**: Provide the required portfolio details in the body.

Track DeFi positions across protocols
- **prediction_address_summary**: Provide the address and time range in the body.

Win rate, PnL, and wallet age in prediction markets
- **prediction_categories**: g., Politics, Crypto). Specify the category in the body.

Stats for market categories (Politics, Crypto, etc.)
- **prediction_event_screener**: Use this tool to find markets based on specific criteria.

Browse groups of related prediction markets
- **prediction_market_screener**: Use the body to specify filtering criteria.

Browse and filter all prediction markets
- **prediction_ohlcv**: Specify the market ID and time range in the body.

1-hour price history candles for prediction markets
- **prediction_orderbook**: Provide the market ID in the request body.

Real-time bid/ask depth for prediction markets
- **prediction_pnl_by_address**: Supply the wallet address and time range in the body.

Total PnL for a trader in prediction markets
- **prediction_pnl_by_market**: Include the market ID and time range in the body.

Profitability rankings for a prediction market
- **prediction_position_detail**: Include the market ID and wallet address in the body.

Granular holder positions for prediction markets
- **prediction_top_holders**: Specify the market ID in the request body.

Largest conviction holders in prediction markets
- **prediction_trades_by_address**: Provide the wallet address and time range in the body.

All trades for a specific wallet in prediction markets
- **prediction_trades_by_market**: Pass the market ID and time frame in the request body.

Recent trades for a specific prediction market
- **profiler_counterparties**: Provide the source address in the request body.

Top addresses/entities interacted with
- **profiler_current_balance**: Provide the address and token details in the body.

Current token balances for an address or entity
- **profiler_historical_balances**: Specify the address and date range in the request body.

Historical holding snapshots for an address
- **profiler_labels**: Pass the necessary body payload.

Non-premium labels (ENS, behavioral)
- **profiler_perp_positions**: Include the required body payload.

Real-time Hyperliquid positions
- **profiler_perp_trades**: Supply the necessary body payload.

Hyperliquid trade history
- **profiler_pnl**: Supply the required body payload.

Detailed PnL for a specific address and token
- **profiler_pnl_summary**: Use this tool to get a summary view of profitability.

Aggregate PnL and top profitable tokens
- **profiler_premium_labels**: Supply the required body payload.

All labels including Smart Money
- **profiler_related_wallets**: Provide the source address in the request body.

Wallets related by on-chain behavior
- **profiler_transactions**: Include the address and desired time frame in the body.

Recent blockchain transactions for an address
- **search_general**: Use this tool when general asset identification is required.

Search for tokens and entities by name, symbol, or contract address
- **smart_money_dcas**: Provide the relevant token and time period in the body.

DCA strategies on Jupiter (Solana)
- **smart_money_dex_trades**: Pass the relevant token and time parameters in the body.

Real-time DEX trading activity (last 24h)
- **smart_money_historical_holdings**: Include the asset and date range in the request body.

Daily snapshots of smart money holdings (Beta)
- **smart_money_holdings**: Specify the required token and time frame in the body.

Aggregated token balances held by smart money
- **smart_money_netflow**: Provide the token identifier in the request body.

Net capital flows (inflows vs outflows) for tokens
- **smart_money_perp_trades**: Include the specific asset pair and time range in the body.

Perpetual trading on Hyperliquid
- **tgm_dex_trades**: Specify the token and time range in the body.

Individual DEX transactions for a token
- **tgm_flow_intelligence**: Supply the required body payload.

Segmented flows (Exchanges, Whales, Smart Money)
- **tgm_flows**: Specify the token and time range in the body.

Hourly snapshots of inflows/outflows by category
- **tgm_holders**: Provide the token address and time range in the body.

Top holders with balance change tracking
- **tgm_indicators**: Pass the necessary body payload.

Risk and Reward scores for a token
- **tgm_jup_dca**: Include the token address and time range in the body.

Jupiter DCA orders for a token (Solana)
- **tgm_pnl_leaderboard**: Provide the token address and time range in the body.

Rank traders by profit for a specific token
- **tgm_token_information**: Supply the required body payload.

Metadata, market metrics, and spot trading stats
- **tgm_token_ohlcv**: Supply the required body payload.

Unified price/volume candles (1m to 1M timeframes)
- **tgm_transfers**: Provide the token and time range in the body.

Top token transfers (ERC-20)
- **tgm_who_bought_sold**: Include the token address and time frame in the body.

Summary of net buyers/sellers
- **token_screener**: Pass the required body payload.

Discover trending tokens across chains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nansen (Blockchain Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the token 'PEPE' and show me its details."

**🤖 AI Agent:**
> I've found the PEPE token. It is currently tracked across multiple exchanges. Would you like to see the Smart Money netflow for PEPE in the last 24 hours?

---

**👤 You:**
> "What are the current Smart Money holdings?"

**🤖 AI Agent:**
> Fetching aggregated Smart Money balances... The top holdings currently include WETH, USDC, and LINK. I can provide a detailed breakdown of the balance for any of these tokens.

---

**👤 You:**
> "Show me the PnL summary for address 0x71C7656EC7ab88b098defB751B7401B5f6d8976F."

**🤖 AI Agent:**
> Analyzing PnL for the specified address... This wallet has an aggregate realized profit of $1.2M, with its most profitable trade being in SHIB. Would you like to see the full transaction history?


## ❓ FAQ

**Q: How can I track where Smart Money is moving capital?**
Use the `smart_money_netflow` tool to see net capital flows (inflows vs outflows) for tokens, or `smart_money_holdings` to see aggregated balances held by these sophisticated entities.

**Q: Can I identify the behavior or identity of a specific wallet?**
Yes, use `profiler_labels` or `profiler_premium_labels` to retrieve behavioral tags (like 'Smart Money', 'Heavy DEX User', or ENS names) associated with any blockchain address.

**Q: How do I analyze the performance of a specific address?**
Use `profiler_pnl_summary` to get an aggregate view of profits and losses, or `profiler_pnl` for a detailed breakdown of performance for a specific address and token pair.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nansen-blockchain-analytics](https://vinkius.com/en/ai-agent-connect/nansen-blockchain-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nansen (Blockchain Analytics)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nansen-blockchain-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nansen (Blockchain Analytics)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nansen-blockchain-analytics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

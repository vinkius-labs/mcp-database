# Glassnode (On-chain Data) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glassnode-on-chain-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access institutional-grade on-chain market data for Bitcoin, Ethereum, and 1000+ assets directly from your AI agent.

## Description
Connect your **Glassnode** account to any AI agent to analyze crypto markets with precision. Fetch real-time and historical on-chain metrics, exchange flows, and network health data through natural conversation.

### What you can do

- **Asset Discovery** — List all supported assets and blockchains using `list_assets` to identify available data points.
- **Metric Exploration** — Query thousands of metric paths with `list_metrics` and get detailed documentation on parameters via `get_metric_details`.
- **Time-Series Analysis** — Retrieve historical data for active addresses, exchange balances, and price metrics using `get_metric`.
- **Bulk Data** — Fetch metrics for multiple assets simultaneously with `get_bulk_metric` to compare market trends.
- **Point-in-Time Data** — Access immutable historical snapshots via `get_pit_metric` to eliminate look-ahead bias in backtesting.

### How it works

1. Subscribe to this server
2. Enter your Glassnode API Key
3. Start querying on-chain intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders** — monitor exchange inflows and whale movements without leaving the chat
- **Data Scientists** — pull clean time-series data directly into your analysis environment
- **Financial Analysts** — generate reports on network growth and valuation metrics instantly


## Available Tools (6)
- **get_bulk_metric**: Use a="*" for all assets.

Get bulk metric data for multiple assets
- **get_metric_details**: Get details, allowed parameters, and description for a specific metric
- **get_metric**: Path should be the metric name like "addresses/active_count" or "market/price_usd_close".

Get time-series data for a specific metric
- **get_pit_metric**: Get Point-in-Time (PIT) metric data
- **list_assets**: List all supported assets on Glassnode
- **list_metrics**: Can be filtered by asset, interval, etc.

List all available metric paths on Glassnode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glassnode (On-chain Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported assets on Glassnode."

**🤖 AI Agent:**
> I've retrieved the list of supported assets. Glassnode currently supports over 1,000 assets including BTC, ETH, and various ERC-20 tokens across multiple blockchains like Bitcoin, Ethereum, and Polygon.

---

**👤 You:**
> "Get the 'addresses/active_count' metric for BTC from the last 7 days with a 24h interval."

**🤖 AI Agent:**
> Fetching active address count for Bitcoin... Over the last 7 days, the daily active addresses have fluctuated between 850k and 920k, showing a slight upward trend in network activity.

---

**👤 You:**
> "Show me the details and allowed parameters for the metric path 'market/price_usd_close'."

**🤖 AI Agent:**
> The 'market/price_usd_close' metric provides the daily closing price in USD. It supports intervals from 10m to 1month and is available for almost all listed assets. You can filter by 'since' and 'until' timestamps.


## ❓ FAQ

**Q: How can I find the exact path for a specific metric like 'Active Addresses'?**
Use the `list_metrics` tool with the asset symbol (e.g., 'BTC') to see all available paths, or use `get_metric_details` with a known path to see its full documentation and allowed parameters.

**Q: Can I fetch data for multiple coins at once?**
Yes, use the `get_bulk_metric` tool. You can specify a specific asset or use a wildcard `*` to get data for all supported assets for a specific metric path in a single response.

**Q: What is the difference between standard metrics and Point-in-Time (PIT) metrics?**
Standard `get_metric` returns the most accurate current data (which may include revisions). `get_pit_metric` provides an immutable view of data as it was known at a specific moment, which is essential for backtesting to avoid look-ahead bias.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glassnode-on-chain-data](https://vinkius.com/mcp/glassnode-on-chain-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glassnode (On-chain Data)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glassnode-on-chain-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glassnode (On-chain Data)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glassnode-on-chain-data": {
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

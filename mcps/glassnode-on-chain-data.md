# Glassnode (On-chain Data) MCP Server

Access institutional-grade on-chain market data for Bitcoin, Ethereum, and 1000+ assets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/glassnode-on-chain-data)

## Overview
**Category:** data-analytics
**Tools Count:** 6

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


## Available Tools
- **get_bulk_metric**: Use a="*" for all assets.

Get bulk metric data for multiple assets
- **get_metric_details**: Get details, allowed parameters, and description for a specific metric
- **get_metric**: Path should be the metric name like "addresses/active_count" or "market/price_usd_close".

Get time-series data for a specific metric
- **get_pit_metric**: Get Point-in-Time (PIT) metric data
- **list_assets**: List all supported assets on Glassnode
- **list_metrics**: Can be filtered by asset, interval, etc.

List all available metric paths on Glassnode


## Installation & Usage

To install and use the **Glassnode (On-chain Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glassnode-on-chain-data](https://vinkius.com/mcp/glassnode-on-chain-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

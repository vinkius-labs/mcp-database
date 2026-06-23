# Santiment (On-chain, Social & Dev Metrics for Crypto) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/santiment-on-chain-social-dev-metrics-for-crypto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access deep on-chain, social, and development metrics for thousands of crypto assets directly from your AI agent.

## Description
Connect **Santiment** to your AI agent to unlock institutional-grade crypto market intelligence. Analyze network growth, social sentiment, and developer activity through natural language.

### What you can do

- **Metric Timeseries** — Fetch historical data for metrics like `daily_active_addresses`, `price_usd`, or `network_growth` for any asset slug.
- **Multi-Asset Comparison** — Compare the performance or health of multiple tokens (e.g., Bitcoin vs Ethereum) in a single query.
- **Project Discovery** — List and search through thousands of available crypto projects to find the correct identifiers (slugs).
- **Advanced Filtering** — Identify market opportunities by filtering projects based on specific thresholds, such as finding assets with high developer activity but low price action.

### How it works

1. Subscribe to this server
2. Enter your Santiment API Key
3. Start querying crypto data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Analysts** — Quickly pull on-chain data to validate market hypotheses without writing complex GraphQL queries.
- **Traders** — Monitor social sentiment and whale movements across multiple assets simultaneously.
- **Web3 Developers** — Track development activity and network health of protocols directly from your IDE.


## Available Tools (4)
- **filter_projects_by_metric**: g., top 10 projects with DAA > 1000).

Filter projects based on a specific metric threshold
- **get_metric_multiple_slugs**: Fetch timeseries data for a metric across multiple asset slugs
- **get_metric_timeseries**: g., daily_active_addresses, price_usd) and asset slug (e.g., bitcoin).

Fetch timeseries data for a specific metric and asset slug
- **list_projects**: Use this to find valid slugs for metric queries.

List all available projects and their slugs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Santiment (On-chain, Social & Dev Metrics for Crypto)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the daily active addresses for bitcoin from 2023-10-01 to now."

**🤖 AI Agent:**
> I've retrieved the daily active addresses for Bitcoin. The data shows a peak of 1.2M addresses on October 25th, with a steady average of 950k throughout the period.

---

**👤 You:**
> "Compare the social volume of ethereum and solana for the last 7 days."

**🤖 AI Agent:**
> Comparing social volume: Ethereum maintained a higher baseline, but Solana saw a 40% spike in mentions yesterday following the latest network update.

---

**👤 You:**
> "Find the top 5 projects with the highest developer activity in the last 30 days."

**🤖 AI Agent:**
> Based on developer activity (dev_activity) over the last 30 days, the top 5 projects are: 1. Cardano, 2. Polkadot, 3. Ethereum, 4. Cosmos, and 5. Chainlink.


## ❓ FAQ

**Q: How can I find the correct slug for a specific cryptocurrency?**
You can use the `list_projects` tool. It provides a paginated list of all available assets and their corresponding slugs used for metric queries.

**Q: Can I compare the price of multiple assets at once?**
Yes! Use the `get_metric_multiple_slugs` tool. Just provide the metric (e.g., 'price_usd') and an array of slugs to get a combined timeseries for comparison.

**Q: Is it possible to find projects based on their network activity levels?**
Absolutely. Use the `filter_projects_by_metric` tool to find projects that meet specific criteria, such as having more than 1000 daily active addresses over a certain period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/santiment-on-chain-social-dev-metrics-for-crypto](https://vinkius.com/mcp/santiment-on-chain-social-dev-metrics-for-crypto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Santiment (On-chain, Social & Dev Metrics for Crypto)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `santiment-on-chain-social-dev-metrics-for-crypto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Santiment (On-chain, Social & Dev Metrics for Crypto)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "santiment-on-chain-social-dev-metrics-for-crypto": {
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

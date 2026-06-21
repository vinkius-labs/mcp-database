# EIA Natural Gas — Gas Market Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-natural-gas-gas-market-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eia-natural-gas-gas-market-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eia-natural-gas-gas-market-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Natural gas market data: Henry Hub spot and futures prices, underground storage levels (the weekly report that moves markets), LNG imports/exports, production by state, pipeline flows, and consumption by sector.

## Description
The definitive natural gas data source. From Henry Hub pricing to weekly storage reports, this server covers every aspect of the U.S. natural gas market.

### What you can do
- **Prices** — Henry Hub spot, citygate, wellhead, industrial, and residential prices
- **Storage** — Weekly underground storage levels by region (the Thursday report)
- **Production** — Gross withdrawals, marketed production, shale gas by state
- **Trade** — LNG imports/exports by terminal, pipeline trade with Canada/Mexico
- **Reserves** — Proved reserves and exploration wells
- **Consumption** — By sector: residential, commercial, industrial, electric power

### Who is this for?
Gas traders, LNG analysts, utility planners, pipeline operators, and energy risk managers.


## Available Tools
- **get_natgas_prices**: Henry Hub spot price is the benchmark for North American gas trading.

Get natural gas prices: Henry Hub, citygate, wellhead, industrial, residential
- **get_natgas_summary**: S. natural gas balance: total production, consumption, imports, exports, and storage changes.

Get natural gas supply and demand overview
- **get_natgas_reserves**: Get natural gas proved reserves and exploration data
- **get_natgas_production**: Get natural gas production: gross withdrawals, marketed production
- **get_natgas_trade**: Get natural gas imports, exports, and pipeline flows
- **get_natgas_storage**: The weekly storage report is a major market-moving event for gas trading.

Get underground natural gas storage levels
- **get_natgas_consumption**: By state and nationally.

Get natural gas consumption by sector


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Natural Gas — Gas Market Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the Henry Hub natural gas price?"

**🤖 AI Agent:**
> 🔥 **Henry Hub Natural Gas Spot Price**

Current: $2.84/MMBtu
Previous: $2.71 (+4.8%)
52-week range: $1.52 — $3.45

Henry Hub is the benchmark for North American natural gas pricing.

---

**👤 You:**
> "What is the current natural gas storage level?"

**🤖 AI Agent:**
> 📦 **U.S. Natural Gas Storage**

Working gas: 2,584 Bcf
Net change: +15 Bcf (injection)
5-year avg: 2,321 Bcf
Above avg: +263 Bcf (+11.3%)

| Region | Bcf | vs 5yr |
|--------|-----|--------|
| East | 612 | +8% |
| Midwest | 487 | +12% |
| South Central | 892 | +14% |
| Mountain | 198 | +6% |
| Pacific | 395 | +10% |

---

**👤 You:**
> "How much LNG does the U.S. export?"

**🤖 AI Agent:**
> 🚢 **U.S. LNG Exports**

Latest month: 11.8 Bcf/d
YTD total: 4,307 Bcf
Top destinations: Europe (62%), Asia (28%)

The U.S. became the world's #1 LNG exporter in 2023, surpassing Qatar and Australia.


## Installation & Usage

To install and use the **EIA Natural Gas — Gas Market Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-natural-gas-gas-market-intelligence](https://vinkius.com/mcp/eia-natural-gas-gas-market-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

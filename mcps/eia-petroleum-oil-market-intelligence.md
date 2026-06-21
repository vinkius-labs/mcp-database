# EIA Petroleum — Oil Market Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-petroleum-oil-market-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eia-petroleum-oil-market-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eia-petroleum-oil-market-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Real-time oil market data: WTI and Brent crude prices, gasoline and diesel retail prices, U.S. production, refinery operations, Strategic Petroleum Reserve levels, crude imports by country, and the weekly petroleum status report.

## Description
Connect your AI agent to the heart of the global oil market. EIA Petroleum provides authoritative data from the world's most-watched energy agency.

### What you can do
- **Crude Oil Prices** — WTI Cushing and Brent spot prices, historical and current
- **Retail Fuel Prices** — Gasoline and diesel at the pump, by region and grade
- **U.S. Production** — Crude oil production by state and PAD district
- **Refinery Operations** — Capacity utilization, inputs, and product yields
- **Petroleum Trade** — Imports/exports by country, pipeline and tanker movements
- **Stocks** — Commercial crude and product stocks + Strategic Petroleum Reserve (SPR)
- **Consumption** — Product supplied by type and sector
- **Crude Imports** — Company-level imports by country, API gravity, sulfur content

### Who is this for?
Oil traders, energy analysts, commodity fund managers, refinery operators, logistics companies, and anyone whose decisions depend on petroleum market intelligence.


## Available Tools
- **get_petroleum_prices**: Filter by product, area, and frequency.

Get petroleum product prices: WTI, Brent, gasoline, diesel, heating oil
- **get_petroleum_summary**: S. petroleum supply/demand balance including production, imports, exports, stocks, and consumption. The weekly petroleum status report data.

Get petroleum supply and demand balance
- **get_crude_production**: Get U.S. crude oil production and reserves data
- **get_refinery_operations**: Get refinery capacity, utilization, and processing data
- **get_petroleum_trade**: Get petroleum imports, exports, and movements
- **get_petroleum_stocks**: Get petroleum stocks: commercial + Strategic Petroleum Reserve
- **get_petroleum_consumption**: Get petroleum consumption and sales by product and sector
- **get_crude_imports**: Source: EIA-814.

Get crude oil imports by country, company, type, and grade


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Petroleum — Oil Market Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current WTI crude oil price?"

**🤖 AI Agent:**
> 🛢️ **WTI Crude Oil (Cushing, OK)**

Spot Price: $78.26/barrel
Previous: $77.89 (+0.47%)
Frequency: Daily

30-day range: $74.50 — $82.10
YTD change: +8.3%

Source: EIA Petroleum Price Survey

---

**👤 You:**
> "How much crude oil does the U.S. import from Saudi Arabia?"

**🤖 AI Agent:**
> 🇸🇦 **U.S. Crude Imports from Saudi Arabia**

Latest month: 342,000 barrels/day
12-month avg: 385,000 bbl/d
API Gravity: 31.2° (medium)
Sulfur: 1.8% (sour)

Saudi Arabia is the #3 source of U.S. crude imports, behind Canada and Mexico.

---

**👤 You:**
> "What is the current level of the Strategic Petroleum Reserve?"

**🤖 AI Agent:**
> 🏛️ **Strategic Petroleum Reserve (SPR)**

Current: 372 million barrels
Capacity: 714 million barrels
Utilization: 52%

The SPR hit a 40-year low in 2023 after emergency releases. The DOE has been slowly refilling at ~$70-77/barrel.


## Installation & Usage

To install and use the **EIA Petroleum — Oil Market Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-petroleum-oil-market-intelligence](https://vinkius.com/mcp/eia-petroleum-oil-market-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

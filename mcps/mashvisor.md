# Mashvisor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mashvisor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mashvisor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mashvisor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Analyze real estate investments — compare Airbnb vs traditional rental ROI via AI.

## Description
Connect **Mashvisor** real estate analytics to any AI agent and analyze investment properties with detailed Airbnb vs traditional rental comparisons, neighborhood analytics, and market insights through natural language.

### What you can do

- **Property Search** — Find investment properties by city, state, price range, and bedrooms
- **Investment Metrics** — Get cap rates, cash-on-cash returns, and revenue projections for both STR and LTR strategies
- **Airbnb Analysis** — View occupancy rates, average daily rates, monthly revenue, and seasonality data
- **Rental Estimates** — Get long-term rental rate estimates for 1-5 bedroom properties
- **Neighborhood Insights** — Compare neighborhoods by ROI, demand indicators, and market benchmarks
- **Market Listings** — Browse active, distressed, and off-market properties in any city
- **Historical Data** — Analyze up to 36 months of Airbnb performance trends

### How it works

1. Subscribe to this server
2. Enter your Mashvisor API Key
3. Start analyzing real estate investments from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_airbnb_listings**: Get Airbnb rental listings and metrics
- **get_airbnb_property**: Get detailed Airbnb listing information
- **get_city_listings**: Filter by status, days on market, price history, and property attributes.

Get city market listings
- **get_historical_performance**: Useful for analyzing seasonality and long-term performance patterns.

Get historical Airbnb performance data
- **get_investment_analysis**: Get property investment analysis
- **get_property**: Get detailed property information
- **get_rental_rates**: Includes rent distribution statistics and helps evaluate traditional rental investment potential.

Get traditional rental rate estimates
- **list_neighborhoods**: List neighborhoods with investment data
- **list_properties**: Filter by city, state, bedrooms, and property type. Returns properties with Airbnb and long-term rental metrics.

List investment properties
- **search_properties**: Returns properties with investment metrics.

Search properties with advanced filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mashvisor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me investment properties in Las Vegas with good Airbnb ROI."

**🤖 AI Agent:**
> Found 15 properties in Las Vegas. Top pick: 3BR/2BA Single Family at $435K with 11.2% cash-on-cash return on Airbnb (73% occupancy, $188/night, $4,124/mo revenue). Traditional rental would yield 5.3% CoC at $2,100/mo.

---

**👤 You:**
> "What's the best neighborhood for Airbnb in Chicago?"

**🤖 AI Agent:**
> Top neighborhoods in Chicago by Airbnb ROI: 1) Logan Square — 8.9% ROI, avg $2,800/mo revenue, 71% occupancy. 2) Wicker Park — 8.2% ROI, $3,100/mo, 68% occupancy. 3) Lincoln Park — 7.5% ROI, $3,400/mo, 65% occupancy.

---

**👤 You:**
> "What are typical rental rates for a 3BR in Austin, TX?"

**🤖 AI Agent:**
> Austin, TX rental estimates: 1BR: $1,400/mo | 2BR: $1,750/mo | 3BR: $2,100/mo | 4BR: $2,600/mo | 5BR: $3,200/mo. The 3BR average is based on 1,200+ comparable rentals in the area.


## Installation & Usage

To install and use the **Mashvisor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mashvisor](https://vinkius.com/mcp/mashvisor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# RentCast MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rentcast)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rentcast-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rentcast-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Automate real estate data and valuation tracking via RentCast — manage properties, rental yields, and market trends directly from any AI agent.

## Description
Connect your **RentCast** account to any AI agent and simplify your real estate investment analysis and property data orchestration through natural conversation.

### What you can do

- **Property Intelligence** — Fetch complete records for any US address, including owner info, tax history, and structural details
- **Rent & Sale AVMs** — Generate real-time rental price estimates and property valuations using advanced market models
- **Market Trends** — Query aggregate trends for any ZIP code, including average rents, occupancy rates, and occupancy levels
- **Rental Listings** — Access current active rental listings to understand local competition and inventory
- **Investment Tracking** — Monitor your portfolio values and local market conditions directly from your agent

### How it works

1. Subscribe to this server
2. Enter your RentCast API Key from your developer dashboard
3. Start managing your real estate data from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_property_by_id**: Get property details by ID
- **get_rental_comparables**: Get comparable rental properties
- **get_sale_comparables**: Get comparable sale properties
- **get_property_details**: Get property data by address
- **get_rental_valuation**: Get rental price estimate (AVM)
- **get_sale_valuation**: Get property sale valuation
- **list_market_trends**: Get market trends by ZIP code
- **list_active_listings**: List active rental listings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RentCast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get property details for 123 Main St, Los Angeles, CA."

**🤖 AI Agent:**
> I've retrieved the records for 123 Main St. It's a Single Family home built in 1995 with 3 beds and 2 baths.

---

**👤 You:**
> "Get the rental valuation and comparable properties for 123 Oak Street, Austin, TX 78701."

**🤖 AI Agent:**
> Rental valuation for 123 Oak Street, Austin, TX 78701. Estimated monthly rent: $2,850. Range: $2,600-$3,100. Property: 3 bed/2 bath, 1,850 sqft, built 2008. 8 comparable rentals found within 0.5 miles. Closest comp: 145 Oak Street ($2,900/mo, 3/2, 1,900 sqft). Market trend: Austin rents up 4.2% YoY. Vacancy rate: 5.8%. Days on market average: 18. Neighborhood grade: A-. Rent-to-price ratio: 0.62% (investor-friendly).

---

**👤 You:**
> "Show me the real estate market trends for ZIP code 78701 over the last 12 months."

**🤖 AI Agent:**
> Market trends for ZIP 78701 (Austin, TX). Median home price: $485,000 (+6.8% YoY). Median rent: $2,450 (+4.2% YoY). Sales volume: 234 homes sold (down 12% from last year). Average days on market: 28 (up from 21). Inventory: 1.8 months supply (seller's market). Price per sqft: $312. Foreclosure rate: 0.3%. New listings this month: 45. Price reductions: 18% of listings. Most active segment: $400K-$600K range.


## Installation & Usage

To install and use the **RentCast** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rentcast](https://vinkius.com/mcp/rentcast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

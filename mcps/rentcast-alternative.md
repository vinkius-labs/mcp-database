# RentCast MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rentcast-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rentcast-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rentcast-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access real-time real estate data, property records, and rental market analytics directly from your AI agent.

## Description
Connect **RentCast** to your AI agent to unlock powerful real estate insights. Query millions of property records, track active listings, and analyze market trends using natural language.

### What you can do

- **Property Records** — Retrieve detailed data on specific properties including square footage, year built, and lot size using `get_property_records`.
- **Sale & Rental Listings** — Search for active or historical listings for sale or rent across the US with `get_sale_listings` and `get_rental_listings`.
- **Market Statistics** — Get aggregated market data to understand local real estate trends via `get_market_stats`.
- **Rental Valuations (AVM)** — Estimate long-term and short-term rental income for any property address using `get_rental_avm_long_term` and `get_rental_avm_short_term`.

### How it works

1. Subscribe to this server
2. Enter your RentCast API Key
3. Start analyzing real estate data from Claude, Cursor, or any MCP client.

### Who is this for?

- **Real Estate Investors** — quickly evaluate potential deals and rental yields.
- **Property Managers** — monitor local market rents and listing competition.
- **Data Analysts** — pull property metadata and market trends directly into your workflow.


## Available Tools
- **get_rental_avm_long_term**: Generate rental valuations and estimated market rents for long-term rentals
- **get_rental_avm_short_term**: Generate rental valuations and estimated market rents for short-term/Airbnb rentals
- **get_market_stats**: Retrieve aggregate market data and trends for a specific zip code
- **get_property_records**: Retrieve detailed information about specific properties or search for property records
- **get_rental_listings**: Search for active and historical rental listings
- **get_sale_listings**: Search for active and historical real estate sale listings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RentCast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 3-bedroom houses for sale in Austin, TX with a price under $500,000."

**🤖 AI Agent:**
> I've found several active listings in Austin matching your criteria. For example, a property at [Address] is listed for $485,000 with 3 beds and 2 baths. Would you like more details on these listings?

---

**👤 You:**
> "What is the estimated monthly rent for 5500 Grand Lake St, Bellaire, TX?"

**🤖 AI Agent:**
> Using the RentCast AVM, the estimated long-term monthly rent for this property is approximately $3,250. This is based on comparable rentals in the area. Should I look up the specific comps used for this estimate?

---

**👤 You:**
> "Get market statistics for the 90210 zip code."

**🤖 AI Agent:**
> For zip code 90210, the median sale price is currently [Price] with an average of [Days] days on market. Rental yields in this area average [Percentage]. Would you like to see how this compares to last quarter?


## Installation & Usage

To install and use the **RentCast** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rentcast-alternative](https://vinkius.com/mcp/rentcast-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

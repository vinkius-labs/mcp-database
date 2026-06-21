# Zoopla MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoopla)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoopla-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoopla-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access real-time UK property market data — search listings, analyze sold prices, and explore local area statistics directly through your AI agent.

## Description
Connect your **Zoopla** API to any AI agent to unlock comprehensive UK real estate insights. From property hunting to market analysis, manage your real estate research through natural conversation.

### What you can do

- **Property Listings** — Search for properties for sale or rent across the UK with filters for price, bedrooms, and property type.
- **Market Valuation** — Access the Zed-Index to find average property values in specific towns, counties, or outcodes.
- **Sales History** — Retrieve average sold prices to understand market trends and historical performance in target areas.
- **Area Insights** — Discover the most and least expensive streets (Rich List) and view local info graphs for crime, education, and demographics.
- **Local Statistics** — Get visual data URLs for local area graphs to better understand the neighborhood profile.

### How it works

1. Subscribe to this server
2. Enter your Zoopla API Key
3. Start querying the UK property market from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Investors** — quickly analyze average sold prices and market trends to identify high-yield opportunities.
- **Home Buyers** — filter listings by specific criteria and research neighborhood statistics without leaving the chat.
- **Data Analysts** — extract property rich lists and Zed-Index values for market reporting and competitive analysis.


## Available Tools
- **average_sold_prices**: Retrieve average sold prices for a particular area
- **local_info_graphs**: Retrieve URLs for graphs showing local area statistics
- **property_listings**: Retrieve a list of properties for sale or to rent in a given area
- **property_rich_list**: Retrieve the most expensive and least expensive streets in a given area
- **zed_index**: Retrieve the Zoopla Zed-Index (average property value) for a specific area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoopla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 3-bedroom houses for sale in London between £500,000 and £800,000."

**🤖 AI Agent:**
> I'm searching Zoopla for 3-bedroom houses in London within your price range... I found several listings, including a semi-detached house in Greenwich for £650,000 and a modern terrace in Fulham for £795,000. Would you like more details on any of these?

---

**👤 You:**
> "What is the average sold price in the SW1 area?"

**🤖 AI Agent:**
> Fetching average sold prices for SW1... According to Zoopla, the average sold price in the SW1 outcode over the last period was approximately £1,250,000. This area typically sees high-value transactions due to its central location.

---

**👤 You:**
> "Show me the most expensive streets in Manchester and any local info graphs available."

**🤖 AI Agent:**
> Retrieving the Manchester Rich List and local statistics... The most expensive street is currently 'Victoria Park' with an average value of £1.2M. I also have URLs for graphs showing local crime rates and education levels in the area. Would you like me to provide those links?


## Installation & Usage

To install and use the **Zoopla** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoopla](https://vinkius.com/mcp/zoopla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

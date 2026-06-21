# Nestoria MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nestoria)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nestoria-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nestoria-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Search real estate listings globally — find properties to buy or rent across multiple countries with advanced filters.

## Description
Connect to **Nestoria**, the leading property search engine, and find your next home or investment through natural conversation. This server allows any AI agent to query thousands of real estate listings across the UK, Spain, France, Germany, Italy, Brazil, and Australia.

### What you can do

- **Global Property Search** — Search for listings in major markets using city names or specific coordinates.
- **Advanced Filtering** — Narrow down results by price range, number of bedrooms, and property types (houses, flats, etc.).
- **Buy vs. Rent** — Toggle between listings for sale or properties available for long-term rental.
- **Smart Sorting** — Order results by relevance, price (high/low), bedroom count, or the newest listings on the market.
- **Keyword Discovery** — Use specific terms like 'garden', 'pool', or 'renovated' to find properties that match your lifestyle.

### How it works

1. Subscribe to this server
2. (Optional) Provide a User Agent string for API identification
3. Start searching for properties directly from Claude, Cursor, or any MCP client

Stop jumping between dozens of real estate portals. Your AI agent can now aggregate and filter the best deals for you.

### Who is this for?

- **Home Buyers & Renters** — quickly find properties that meet specific criteria without manual searching
- **Real Estate Investors** — monitor market trends and new listings in specific regions
- **Relocation Specialists** — help clients find housing in new countries using localized search data


## Available Tools
- **search_listings**: Search for real estate listings on Nestoria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nestoria** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for houses to buy in London with at least 3 bedrooms."

**🤖 AI Agent:**
> I've found several houses in London with 3+ bedrooms. For example, a Victorian terrace in Fulham for £1,250,000 and a modern house in Greenwich. Would you like to see more details on these?

---

**👤 You:**
> "Find apartments for rent in Madrid between 1000 and 2000 euros."

**🤖 AI Agent:**
> Searching Nestoria Spain... I found 12 apartments in Madrid within your budget. Most are located in the Centro and Chamberí districts. Should I list them by price or newest first?

---

**👤 You:**
> "Look for properties in Paris with the keyword 'garden'."

**🤖 AI Agent:**
> I've filtered listings in Paris for 'garden'. I found a beautiful ground-floor flat in the 16th arrondissement and a house in Montmartre with a private courtyard. Would you like the full descriptions?


## Installation & Usage

To install and use the **Nestoria** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nestoria](https://vinkius.com/mcp/nestoria)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

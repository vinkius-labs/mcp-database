# Bridge Data Output MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bridge-data-output)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bridge-data-output-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bridge-data-output-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access standardized real estate data via the Bridge API — browse MLS listings, property details, and agent info directly from any AI agent.

## Description
Connect your **Bridge Interactive (Zillow Group)** account to any AI agent and orchestrate your real estate research, listing analysis, and market data workflows through natural conversation.

### What you can do

- **Listing Oversight** — Browse thousands of real estate listings (properties) from various MLS datasets with advanced OData filtering.
- **Property Deep Dives** — Retrieve detailed metadata for specific properties, including physical characteristics and historical values.
- **Directory Access** — List real estate members (agents) and offices associated with specific datasets.
- **Media Management** — Access links to high-resolution photos, virtual tours, and media associated with property listings.
- **Market Analysis** — Search for properties by city, price range, or recent modifications to track market trends.
- **Dataset Discovery** — List all available data systems (MLSs) your application has access to.

### How it works

1. Subscribe to this server
2. Enter your Bridge Server Token (Bearer)
3. Start exploring real estate markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Analysts** — quickly gather listing data for market reports without manual dashboard exports.
- **App Developers** — verify data structures and query logic using natural language.
- **Investment Teams** — monitor specific areas and price ranges for new opportunities.


## Available Tools
- **get_dataset_metadata**: Get schema metadata for a specific dataset
- **get_property**: Get details of a specific property
- **list_data_systems**: List all available real estate data systems (MLSs)
- **list_media**: List media (photos/videos) from a dataset
- **list_members**: List real estate agents (members) from a dataset
- **list_offices**: List real estate offices from a dataset
- **list_properties**: List properties from a specific dataset
- **list_recent_listings**: List the most recently modified properties
- **search_properties_by_city**: Search for properties in a specific city
- **search_properties_by_price**: Search for properties above a specific price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bridge Data Output** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all real estate data systems I can access."

**🤖 AI Agent:**
> I've retrieved your data systems. You have access to several sources, including 'Miami Realtors MLS' (ID: miami_mls) and 'Zillow Property Feed' (ID: zillow_data).

---

**👤 You:**
> "Search for properties in Miami with a price over $1,000,000."

**🤖 AI Agent:**
> Retrieving listings in Miami... I found 10 properties above $1M, including a 4-bed condo on Brickell Ave ($1.2M) and a waterfront estate ($3.5M). Would you like full details for any of these?

---

**👤 You:**
> "Get details for property listing key 12345-6789."

**🤖 AI Agent:**
> Property 12345-6789 is a Single Family Home located at 742 Evergreen Terrace. It features 3 bedrooms, 2 bathrooms, 2,500 sqft, and was last modified on March 20th.


## Installation & Usage

To install and use the **Bridge Data Output** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bridge-data-output](https://vinkius.com/mcp/bridge-data-output)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

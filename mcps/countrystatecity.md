# CountryStateCity MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/countrystatecity)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/countrystatecity-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/countrystatecity-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access global geographic data — list countries, states, and cities with ISO codes and metadata directly from any AI agent.

## Description
Connect the **CountryStateCity** database to your AI agent and instantly retrieve accurate geographic data through natural conversation.

### What you can do

- **Global Country List** — Retrieve all countries with their ISO2/ISO3 codes, phone codes, and emojis
- **State & Province Discovery** — List all administrative divisions (states, provinces, regions) for any specific country
- **City Level Granularity** — Drill down into specific cities within a state or fetch all cities in a country (Supporter+ tier)
- **Detailed Metadata** — Access specific fields like latitude, longitude, and currency for precise location context

### How it works

1. Subscribe to this server
2. Enter your CountryStateCity API Key
3. Start querying global locations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly find ISO codes and regional IDs without leaving the code editor
- **Data Analysts** — validate geographic hierarchies and clean location data via chat
- **Logistics & E-commerce** — verify shipping regions and city-state relationships instantly


## Available Tools
- **get_country**: Get details for a specific country
- **get_state**: Get details for a specific state
- **list_cities_by_country**: Note: Requires Supporter+ tier.

List all cities within a specific country
- **list_cities_by_state**: List all cities within a specific state
- **list_countries**: List all countries
- **list_states**: List all states/provinces within a specific country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CountryStateCity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all countries and include their emojis."

**🤖 AI Agent:**
> I've retrieved the list of countries. Here are a few: Afghanistan (AF) 🇦🇫, Albania (AL) 🇦🇱, Algeria (DZ) 🇩🇿, and Andorra (AD) 🇦🇩. Would you like the full list or details for a specific one?

---

**👤 You:**
> "What are the states in India (IN)?"

**🤖 AI Agent:**
> Querying states for India... I found 36 states/territories, including Maharashtra (MH), Delhi (DL), Karnataka (KA), and Tamil Nadu (TN). Which state would you like to explore further?

---

**👤 You:**
> "List the cities in the state of New York (NY), US."

**🤖 AI Agent:**
> Fetching cities for New York, United States... I've found cities such as Albany, Buffalo, New York City, and Rochester. Do you need specific details for any of these cities?


## Installation & Usage

To install and use the **CountryStateCity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/countrystatecity](https://vinkius.com/mcp/countrystatecity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# FNS SNAP Retailer Locator (USDA) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fns-snap-retailer-locator-usda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fns-snap-retailer-locator-usda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fns-snap-retailer-locator-usda-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Locate SNAP-authorized retailers across the US using USDA public data. Filter by location, store name, or coordinates.

## Description
Connect to the **USDA Food and Nutrition Service (FNS)** database to locate retailers authorized to accept SNAP benefits (Supplemental Nutrition Assistance Program) across the United States through natural conversation.

### What you can do

- **Attribute Search** — Filter retailers by State, City, Zip Code, or Store Name using flexible SQL-like queries.
- **Spatial Discovery** — Find all authorized stores within a specific radius (miles or kilometers) of any GPS coordinate.
- **Detailed Metadata** — Retrieve store names, addresses, and geographic locations for thousands of retailers.
- **Pagination Control** — Efficiently browse large sets of results using record offsets and limits.

### How it works

1. Subscribe to this server
2. No API key is required as this server accesses public government data
3. Start searching for food resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Services & Non-profits** — Quickly identify food resources for families and individuals in need.
- **Data Analysts & Researchers** — Study the distribution of SNAP-authorized retailers and identify food deserts.
- **Public Health Officials** — Map food accessibility and coordinate community outreach programs.


## Available Tools
- **search_retailers_by_location**: Search for SNAP-authorized retailers within a radius of a coordinate
- **search_retailers**: Example: State = 'VA' AND Zip5 = '22314'

Search for SNAP-authorized retailers by attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FNS SNAP Retailer Locator (USDA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all SNAP-authorized retailers in zip code 30303."

**🤖 AI Agent:**
> I found several SNAP-authorized retailers in Atlanta (30303), including 'CVS Pharmacy' on Peachtree St and 'Walgreens' on Marietta St. Would you like the full list of addresses?

---

**👤 You:**
> "Search for SNAP stores within 10 miles of latitude 34.05, longitude -118.24."

**🤖 AI Agent:**
> Searching near Los Angeles... I've located 45 authorized retailers within 10 miles of those coordinates. Notable locations include 'Target' on W 7th St and 'Whole Foods Market' on Grand Ave.

---

**👤 You:**
> "List SNAP retailers in Virginia that have 'Market' in their name."

**🤖 AI Agent:**
> Querying retailers in VA with 'Market' in the name... I found entries like 'Union Market' in Richmond and 'Farmers Market' in Alexandria. Do you want to see more results or filter by city?


## Installation & Usage

To install and use the **FNS SNAP Retailer Locator (USDA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fns-snap-retailer-locator-usda](https://vinkius.com/mcp/fns-snap-retailer-locator-usda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

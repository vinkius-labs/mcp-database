# UK ONS Discovery — Search 337+ Statistical Datasets MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-discovery-search-337-statistical-datasets)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uk-ons-discovery-search-337-statistical-datasets-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uk-ons-discovery-search-337-statistical-datasets-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore the full ONS dataset catalog: search 337+ datasets by keyword, browse metadata and dimensions, discover available filter options, and query any dataset with flexible parameters covering every aspect of UK statistics.

## Description
Full access to the ONS dataset catalog with discovery and query tools.

### What you can do
- **Search** — Find datasets by keyword
- **Browse** — Paginated catalog access
- **Metadata** — Dataset details, methodology, contacts
- **Dimensions** — Available filter variables
- **Options** — Valid values for each dimension
- **Query** — Flexible observations with dimension filters


## Available Tools
- **search_datasets**: Returns matching dataset IDs, titles, and descriptions. Use this to find the right dataset before querying data.

Search ONS datasets by keyword — explore 337+ available datasets
- **list_datasets**: The catalog contains 337+ datasets covering economy, population, health, trade, business, and more.

Browse the complete ONS dataset catalog with pagination
- **get_dataset_info**: Get metadata for an ONS dataset: dimensions, editions, versions
- **get_dimensions**: Each dimension has options you can use to filter observations. Essential for understanding what query parameters to use.

Get available dimensions and filter options for an ONS dataset
- **get_dimension_options**: g., all geography codes, all time periods, all aggregate categories). Use this to find the correct filter values for observations.

Get all option values for a specific dimension in an ONS dataset
- **get_observations**: Provide dataset ID and dimension filters. Use search_datasets to find IDs and get_dimensions to discover available filters. Set time=* for full time series.

Query any ONS dataset by ID with flexible dimension filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK ONS Discovery — Search 337+ Statistical Datasets** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What ONS datasets are available about housing?"

**🤖 AI Agent:**
> 🔍 **ONS Datasets: housing**

1. house-prices-local-authority — House prices by local authority
2. housing-stock — Dwelling stock estimates
3. new-build — New house building statistics
4. private-rent — Private rental market statistics

4 datasets found matching 'housing'.

---

**👤 You:**
> "Can you list the variables (dimensions) available for the house-prices dataset?"

**🤖 AI Agent:**
> The 'house-prices-local-authority' dataset has 3 dimensions you can filter by:
1. 'geography' (e.g., specific councils/authorities)
2. 'property-type' (e.g., detached, flat, semi-detached)
3. 'time' (year and month).

---

**👤 You:**
> "What is the latest data on the UK employment rate?"

**🤖 AI Agent:**
> I found the 'employment-rate' dataset. Filtering for the latest quarter, the estimated UK employment rate for people aged 16 to 64 was 74.8%, which is a slight increase from the previous quarter.


## Installation & Usage

To install and use the **UK ONS Discovery — Search 337+ Statistical Datasets** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-discovery-search-337-statistical-datasets](https://vinkius.com/mcp/uk-ons-discovery-search-337-statistical-datasets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

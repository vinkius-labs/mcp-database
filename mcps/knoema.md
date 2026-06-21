# Knoema MCP Server

Access global statistics — search datasets, retrieve time-series data, and audit economic indicators.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/knoema)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect your AI agent to **Knoema**, the most comprehensive source of global decision-making data.

### What you can do

- **Dataset Discovery** — Search through millions of datasets from official sources like IMF, World Bank, and UN
- **Data Retrieval** — Fetch precise time-series data using mnemonics for your analysis and forecasting
- **Metadata Auditing** — Get detailed information about data sources, units, and frequencies
- **Granular Search** — Find specific indicators (e.g., GDP, CPI, Crude Oil Price) across multiple providers
- **Visualization Support** — Access atlas and dashboard resources for visual data context

### How it works

1. Subscribe to this server
2. Enter your Knoema Client ID and Secret (from the Developer Portal)
3. Start querying global statistics directly from your chat client

### Use Cases

- **Economic Analysis** — gather historical and current macro indicators for market research
- **Business Planning** — use demographic and sector data to inform strategy
- **Scientific Research** — find environmental and social datasets for academic or professional studies


## Available Tools
- **search_datasets**: Returns dataset IDs and metadata. Use this to find the correct data source for your statistics.

Search for datasets in Knoema
- **get_dataset_metadata**: Critical for understanding what variables are available.

Get metadata for a specific dataset
- **list_data_topics**: g., Agriculture, Economy, Demographics).

List all available data topics in Knoema
- **get_data_series**: Requires dataset ID and a list of mnemonics.

Get specific data series
- **list_dataset_regions**: ) supported by a specific dataset.

List regions available in a dataset
- **list_data_units**: g., Percentage, USD, Kilograms).

List measurement units
- **get_latest_dataset_data**: Get the most recent data points for a dataset
- **search_data_series**: More granular than dataset search. Ideal for finding specific indicators.

Search for specific data series across all datasets
- **list_data_frequencies**: g., Annual, Quarterly, Monthly).

List available data frequencies
- **get_knoema_resource**: Get a generic frontend resource


## Installation & Usage

To install and use the **Knoema** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knoema](https://vinkius.com/mcp/knoema)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

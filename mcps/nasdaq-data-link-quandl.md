# Nasdaq Data Link (Quandl) MCP Server

Access financial, economic, and alternative data from Nasdaq Data Link. Query datatables, fetch metadata, and manage bulk downloads directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nasdaq-data-link-quandl)

## Overview
**Category:** money-moves
**Tools Count:** 4

## Description
Connect your **Nasdaq Data Link** (formerly Quandl) account to any AI agent to access professional-grade financial and economic datasets through natural language.

### What you can do

- **Datatable Queries** — Fetch unsorted data from specific vendors and tables with advanced filtering for tickers, dates, and more
- **Metadata Inspection** — Retrieve table descriptions, column types, and identify which columns are filterable before running large queries
- **Bulk Data Management** — Initiate bulk downloads for entire datasets or large slices, returning status updates (PENDING, RUNNING, SUCCEEDED)
- **File Retrieval** — Download specific bulk files in CSV, Parquet, or ZIP formats once exports are processed
- **Pagination & Exporting** — Handle large result sets using cursor-based pagination or trigger direct exports for external analysis

### How it works

1. Subscribe to this server
2. Enter your Nasdaq Data Link API Key
3. Start querying financial markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly pull historical prices or alternative data without writing complex API scripts
- **Data Scientists** — explore dataset schemas and initiate bulk exports directly from your research environment
- **Quantitative Researchers** — automate the retrieval of economic indicators and fundamental data for model inputs


## Available Tools
- **request_bulk_download**: Returns a status (PENDING, RUNNING, SUCCEEDED) and file URLs.

Request a bulk download for a datatable
- **get_bulk_download_file**: Download a specific bulk file
- **get_datatable**: Use filters to narrow down results.

Get unsorted data from a Nasdaq datatable
- **get_datatable_metadata**: Get metadata for a Nasdaq datatable


## Installation & Usage

To install and use the **Nasdaq Data Link (Quandl)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasdaq-data-link-quandl](https://vinkius.com/mcp/nasdaq-data-link-quandl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

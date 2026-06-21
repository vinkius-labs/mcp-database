# Nasdaq Data Link (Quandl) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasdaq-data-link-quandl)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasdaq-data-link-quandl-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasdaq-data-link-quandl-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Access financial, economic, and alternative data from Nasdaq Data Link. Query datatables, fetch metadata, and manage bulk downloads directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nasdaq Data Link (Quandl)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the metadata for the MER/F1 datatable."

**🤖 AI Agent:**
> I've retrieved the metadata for MER/F1. This table contains fundamental financial data. Available columns include 'reportid', 'unitid', 'indicatorid', and 'value'. The columns 'ticker' and 'date' are primary filters.

---

**👤 You:**
> "Fetch the latest 5 records from WIKI/PRICES for ticker MSFT."

**🤖 AI Agent:**
> Querying WIKI/PRICES for MSFT... I found the most recent data points. On 2018-03-27, the close price was 89.47. Would you like me to export the full history for this ticker?

---

**👤 You:**
> "Request a bulk download for the ZACKS/CP datatable."

**🤖 AI Agent:**
> I have initiated the bulk download request for ZACKS/CP. The current status is 'PENDING'. I will monitor the export and let you know when the file is ready for download.


## Installation & Usage

To install and use the **Nasdaq Data Link (Quandl)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasdaq-data-link-quandl](https://vinkius.com/mcp/nasdaq-data-link-quandl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Import.io (Web Data Extraction) MCP Server

Extract structured data from any website via Import.io — run extractors, manage bulk crawls, and monitor API usage.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/importio-web-data-extraction)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Import.io** account to any AI agent and take full control of your web data extraction and large-scale scraping through natural conversation.

### What you can do

- **Precision Extraction** — Trigger predefined extractors for specific URLs to retrieve clean, structured JSON data directly from your agent
- **Bulk Crawling** — Start large-scale data extraction jobs across multiple pages concurrently using managed crawlers and monitor their progress in real-time
- **AI-Powered Magic API** — Automatically identify and extract tabular data from any website without pre-configured extractors, perfect for rapid exploration
- **Status Monitoring** — Poll ongoing extraction runs and crawl jobs to track processing states, success rates, and total pages processed
- **Data Export** — Retrieve extraction results in structured JSON or CSV formats, ready for spreadsheet processing or downstream application logic
- **Usage Audit** — Monitor your monthly API credit consumption and subscription limits to manage your data extraction budget effectively

### How it works

1. Subscribe to this server
2. Enter your Import.io API Key
3. Start extracting web data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — automate the collection of market data and pricing intelligence through natural conversation
- **Market Researchers** — perform large-scale competitor monitoring and web audits without manual scraping scripts
- **Product Managers** — verify data extraction schemas and monitor crawler health across multiple projects efficiently


## Available Tools
- **get_crawl_data**: Retrieve the unified JSON output of a completed import.io crawl job
- **get_crawl_status**: start_crawl to check progress (pages processed, success rate, current state).

Check the status of an ongoing import.io crawl job
- **download_csv**: Returns the first 1000 characters and file stats. Ideal for spreadsheet processing.

Download extraction data directly as CSV text
- **get_extractor_data**: Fails if the run is still in progress.

Retrieve structured JSON data from a completed import.io extraction
- **list_extractors**: Useful for finding the correct extractor_id to run dynamically.

List all extractors configured on the import.io account
- **run_magic_api**: Ideal for quick, unstructured exploration.

Run the import.io automated Magic API against a URL
- **run_extractor**: Triggers an async extraction run and returns a run_id. Use this run_id to poll for status or data.

Trigger an import.io extractor for a specific URL
- **start_crawl**: Starts a large-scale data extraction job across multiple pages concurrently.

Trigger an import.io bulk crawl job
- **get_extractor_status**: run_extractor. Returns the current state (running, completed, failed) and metadata about the run.

Check the status of an active or past import.io extraction run
- **account_usage**: No parameters required.

Check import.io account API credit usage


## Installation & Usage

To install and use the **Import.io (Web Data Extraction)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/importio-web-data-extraction](https://vinkius.com/mcp/importio-web-data-extraction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

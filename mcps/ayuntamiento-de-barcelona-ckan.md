# Ayuntamiento de Barcelona (CKAN) MCP Server

Access the Open Data BCN portal to query urban datasets, environmental records, and public statistics directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect to the **Ayuntamiento de Barcelona (Open Data BCN)** portal and transform public data into actionable insights through natural conversation. This MCP server leverages the CKAN API to provide real-time access to Barcelona's official data repository.

### What you can do

- **Dataset Discovery** — List all available datasets or search for specific topics like transportation, environment, or demographics using `bcn_package_search`.
- **Metadata Inspection** — Retrieve detailed metadata for specific datasets and resources to understand data structures and update frequencies.
- **Deep Data Querying** — Use `bcn_datastore_search` to filter records within CSV resources or execute complex `bcn_datastore_search_sql` queries for precise data extraction.
- **Resource Management** — List all resources associated with a dataset, including download links and format specifications.

### How it works

1. Subscribe to this server
2. Enter your Open Data BCN API Token (optional for public data, required for higher rate limits)
3. Start querying Barcelona's public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — Quickly fetch and filter urban data without manual CSV downloads.
- **Urban Planners** — Access real-time statistics on city infrastructure and services.
- **Developers** — Integrate official city data into applications using SQL-like queries directly from the AI.


## Available Tools
- **bcn_current_packages**: List datasets including their resources
- **bcn_datastore_search_sql**: The table name must be the resource_id wrapped in double quotes.

Execute SQL queries directly against a resource
- **bcn_datastore_search**: Search and filter records within a specific CSV resource
- **bcn_package_list**: List all dataset names in the Open Data BCN catalogue
- **bcn_package_search**: Search for datasets matching specific criteria
- **bcn_package_show**: Get metadata for a specific dataset
- **bcn_resource_show**: Get metadata for a specific resource


## Installation & Usage

To install and use the **Ayuntamiento de Barcelona (CKAN)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan](https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

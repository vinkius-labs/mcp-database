# Ayuntamiento de Barcelona (CKAN) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ayuntamiento-de-barcelona-ckan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ayuntamiento-de-barcelona-ckan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the Open Data BCN portal to query urban datasets, environmental records, and public statistics directly through AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ayuntamiento de Barcelona (CKAN)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 datasets available in the Barcelona Open Data catalogue."

**🤖 AI Agent:**
> I've retrieved the first 10 datasets. They include 'arbrat-zona' (Tree zones), 'estacions-meteorologiques' (Weather stations), and 'mercats-municipals' (Municipal markets). Would you like to see the resources for any of these?

---

**👤 You:**
> "Search for datasets about 'wifi' in Barcelona and show their descriptions."

**🤖 AI Agent:**
> I found 3 datasets related to 'wifi'. The main one is 'punts-wifi', which contains the locations of all public WiFi hotspots in the city. It includes resources in CSV, JSON, and KML formats.

---

**👤 You:**
> "Run a SQL query to get the count of records in resource '2023-accidents-gu-bcn'."

**🤖 AI Agent:**
> The SQL query `SELECT count(*) from "2023-accidents-gu-bcn"` returned a total of 8,452 records for traffic accidents in 2023. Would you like to filter these by district?


## Installation & Usage

To install and use the **Ayuntamiento de Barcelona (CKAN)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan](https://vinkius.com/mcp/ayuntamiento-de-barcelona-ckan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

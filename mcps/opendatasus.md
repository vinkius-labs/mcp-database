# OpenDataSUS MCP Server

Access Brazilian public health data (SUS) directly from your AI. Query datasets, search resources, and analyze health statistics from the official portal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opendatasus)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to the **OpenDataSUS** portal to explore and analyze Brazilian public health information through natural language. This server interfaces with the CKAN-based API of the Ministry of Health.

### What you can do

- **Dataset Discovery** — List all available datasets, search for specific health topics (like COVID-19 or vaccination), and browse by tags or categories.
- **Metadata Inspection** — Retrieve detailed metadata for packages and individual resources to understand data provenance and structure.
- **Deep Data Querying** — Use the DataStore search to filter and retrieve actual rows from CSV and Excel resources directly into your conversation.
- **Organizational Browsing** — List data providers and organizations to find specific departmental records.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OpenDataSUS API Key for higher rate limits
3. Start querying Brazilian health data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Scientists & Researchers** — quickly find and sample epidemiological data without manual downloads
- **Public Health Analysts** — monitor health indicators and dataset updates through simple queries
- **Developers** — integrate official Brazilian health data into applications and dashboards with ease


## Available Tools
- **datastore_search**: Search and filter data within a resource
- **group_list**: List all groups (categories)
- **organization_list**: List all organizations (data providers)
- **package_list**: List all dataset names in the OpenDataSUS portal
- **package_search**: Search for datasets matching specific criteria
- **package_show**: Get full metadata of a specific dataset
- **resource_show**: Get metadata for a specific resource
- **tag_list**: List all tags used across datasets


## Installation & Usage

To install and use the **OpenDataSUS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opendatasus](https://vinkius.com/mcp/opendatasus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

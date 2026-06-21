# CVM Dados Abertos MCP Server

Access Brazilian capital markets data directly from the CVM Open Data portal — query investment funds, listed companies, and financial reports.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cvm-dados-abertos)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Connect your AI agent to the **CVM (Comissão de Valores Mobiliários)** Open Data portal and explore the Brazilian financial market through natural conversation.

### What you can do

- **Dataset Exploration** — List all available datasets or search for specific topics like 'investment funds' or 'listed companies'.
- **Deep Metadata Inspection** — Fetch complete metadata for specific datasets, including update frequency, tags, and organizational ownership.
- **Resource Access** — Retrieve direct links and metadata for specific data resources (CSV, XML, or PDF files) within the portal.
- **Organizational Mapping** — List the CVM departments and thematic groups responsible for publishing specific sets of financial data.
- **Market Research** — Quickly find registration data (fi-cad) or daily reports (infodiario) without navigating complex web directories.

### How it works

1. Subscribe to this server
2. Enter your CVM API Key (optional for public access, but recommended for higher limits)
3. Start querying Brazilian financial data from Claude, Cursor, or any MCP client

### Who is this for?

- **Financial Analysts** — instantly find the latest registration data for investment funds or corporate filings.
- **Data Scientists** — automate the discovery of CSV resources for financial modeling and market analysis.
- **Compliance Officers** — verify organizational data and thematic groupings for regulatory reporting.


## Available Tools
- **list_groups**: g., "Fundos de Investimento", "Companhias").

List thematic groups
- **list_organizations**: g., CVM departments) that publish data on the portal.

List organizations that publish data
- **list_datasets**: List all datasets available on the CVM portal
- **search_datasets**: Search for datasets matching specific criteria
- **get_dataset**: Get complete metadata for a specific dataset
- **get_resource**: Get metadata for a specific resource


## Installation & Usage

To install and use the **CVM Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cvm-dados-abertos](https://vinkius.com/mcp/cvm-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

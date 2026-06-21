# TED EU MCP Server

Search EU public procurement tenders via TED — find contracts by country, sector, or value range from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ted-eu)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Connect **TED (Tenders Electronic Daily)** to any AI agent and search EU public procurement opportunities through natural conversation instead of navigating complex procurement portals.

### What you can do

- **Full-Text Search** — Search across all TED procurement notices using keywords like "software development" or "medical equipment"
- **Country Filtering** — Find active tenders from any of the 27 EU member states using ISO country codes
- **CPV Classification** — Search by Common Procurement Vocabulary codes to target specific industry sectors
- **Value Range Search** — Filter tenders by contract value in EUR to match your company size and capacity
- **Recent Opportunities** — Monitor newly published tenders from the last 7 days to stay ahead of deadlines
- **Notice Details** — Retrieve full procurement details including lots, award criteria, timelines, and contracting authority contacts

### How it works

1. Subscribe to this server
2. Optionally enter a TED API Key for higher rate limits (anonymous access works for basic searches)
3. Start finding procurement opportunities from Claude, Cursor, or any MCP-compatible client

TED is the official publication platform of the European Union for public procurement notices, publishing over 700,000 contract opportunities annually.

### Who is this for?

- **Business Development Teams** — discover relevant government contracts across Europe without manually browsing TED
- **Procurement Consultants** — quickly assess market opportunities for clients in specific sectors or countries
- **Public Affairs Analysts** — monitor procurement trends and spending patterns across EU member states


## Available Tools
- **search_tenders**: Returns title, country, value, deadline, and contracting authority. Covers all 27 EU member states.

Search EU public tenders
- **get_tender**: Includes description, lots, award criteria, timelines, and contracting authority contact.

Get tender notice details
- **search_by_country**: Use ISO country codes: DE, FR, ES, IT, PT, NL, etc.

Search tenders by country
- **search_by_cpv**: CPV codes classify EU contracts by sector: 72000000 (IT), 45000000 (Construction), 33000000 (Medical).

Search tenders by CPV code
- **search_by_value**: Useful for finding contracts matching your company size.

Search tenders by contract value
- **list_recent_tenders**: Default is 7 days. Use to monitor new opportunities.

List recently published tenders


## Installation & Usage

To install and use the **TED EU** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ted-eu](https://vinkius.com/mcp/ted-eu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

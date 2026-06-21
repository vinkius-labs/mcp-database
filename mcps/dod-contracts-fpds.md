# DOD Contracts (FPDS) MCP Server

Search and analyze Department of Defense (DOD) and federal contracts via the FPDS Atom Feed directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dod-contracts-fpds)

## Overview
**Category:** data-analytics
**Tools Count:** 1

## Description
Connect your AI agent to the **Federal Procurement Data System (FPDS)** to monitor government spending and analyze contract awards in real-time.

### What you can do

- **Contract Search** — Query the massive database of federal procurement actions using standard FPDS search syntax.
- **DOD Targeting** — Specifically isolate Department of Defense data by filtering for Department ID '9700' or Agency Code '9700'.
- **Market Intelligence** — Track vendor performance, identify upcoming procurement trends, and analyze historical spending patterns.
- **Pagination Support** — Navigate through large result sets using the start parameter to fetch data in batches of 10.

### How it works

1. Subscribe to this server
2. Configure your access identifier
3. Start querying federal contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Government Contractors** — monitor competitors and find new opportunities within the DOD.
- **Data Analysts** — extract raw XML contract data for spending analysis and reporting.
- **Journalists & Researchers** — track government transparency and public spending across federal agencies.


## Available Tools
- **search_contracts**: To target DOD contracts, include DEPARTMENT_ID:"9700" or AGENCY_CODE:"9700" in the sQuery parameter. Returns XML data containing contract entries.

Search federal contracts via FPDS Atom Feed


## Installation & Usage

To install and use the **DOD Contracts (FPDS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dod-contracts-fpds](https://vinkius.com/mcp/dod-contracts-fpds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

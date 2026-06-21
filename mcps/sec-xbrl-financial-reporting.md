# SEC XBRL (Financial Reporting) MCP Server

Access real-time SEC EDGAR financial data — query filing histories, company facts, and XBRL disclosures directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-xbrl-financial-reporting)

## Overview
**Category:** data-management
**Tools Count:** 4

## Description
Connect your AI agent to the **SEC EDGAR** database and perform deep financial analysis using standardized XBRL data. This server provides programmatic access to the U.S. Securities and Exchange Commission's public filing infrastructure.

### What you can do

- **Filing History** — Retrieve the complete submission history for any entity using its Central Index Key (CIK)
- **Company Facts** — Fetch the entire dictionary of XBRL facts reported by a company, covering all taxonomies (US-GAAP, IFRS, etc.)
- **Concept Analysis** — Drill down into specific financial concepts (e.g., Net Income, Assets) for a single company over time
- **Market-Wide Frames** — Aggregate specific financial data points across all reporting entities for a particular period and unit

### How it works

1. Subscribe to this server
2. Enter your SEC User-Agent string (required by SEC Fair Access policy)
3. Start querying financial statements from Claude, Cursor, or any MCP client

### Who is this for?

- **Financial Analysts** — instantly pull raw XBRL data for modeling without manual spreadsheet entry
- **Investors** — monitor recent filings and compare metrics across industries using standardized frames
- **Compliance Officers** — verify submission histories and disclosure accuracy for specific CIKs


## Available Tools
- **get_company_concept**: Get all XBRL disclosures for a single company concept
- **get_company_facts**: Get all company concepts data for a specific company
- **get_submissions**: Includes metadata and recent filings.

Get filing history for a specific entity
- **get_xbrl_frames**: Get aggregated facts for a specific concept and period


## Installation & Usage

To install and use the **SEC XBRL (Financial Reporting)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-xbrl-financial-reporting](https://vinkius.com/mcp/sec-xbrl-financial-reporting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

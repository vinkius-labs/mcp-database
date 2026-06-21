# CFPB Complaints MCP Server

Search 13.8M+ consumer complaints against financial companies — filter by product, company, state and issue.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cfpb-complaints)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect to **CFPB Consumer Complaint Database** and explore 13.8M+ consumer complaints through natural conversation — no API key needed.

### What you can do

- **Complaint Search** — Search complaints by product, company, state, issue and date range
- **Company Complaints** — View all complaints against a specific company
- **State Complaints** — Browse complaints from a specific US state
- **Product Complaints** — Find complaints for specific financial products (Mortgage, Debt Collection, Credit Card)
- **Consumer Narratives** — Read detailed consumer narratives describing their experiences
- **Recent Complaints** — Track recently filed complaints and complaint trends
- **Statistics** — Get complaint counts for quick analysis

### How it works

1. Subscribe to this server
2. No API key needed — data is open public domain
3. Start exploring complaint data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Consumers** — research company complaint histories before choosing financial products
- **Researchers** — analyze complaint trends, company responses and regulatory patterns
- **Journalists** — find complaint data for investigative reporting on financial companies


## Available Tools
- **get_company_complaints**: Returns complaint details including products, issues, states, dates and company responses.

Get complaints against a specific company
- **get_complaint**: Returns full complaint details including product, company, issue, narrative (if available), dates and company response.

Get a specific complaint by ID
- **get_complaints_by_issue**: Common issues: "Incorrect information", "Problem with a purchase", "Attempts to collect debt not owed".

Get complaints for a specific issue type
- **get_complaints_by_product**: Common products: "Mortgage", "Debt collection", "Credit card", "Student loan", "Credit reporting".

Get complaints for a specific product type
- **get_complaints_by_state**: Returns complaint details including products, companies, issues and dates.

Get complaints from a specific US state
- **get_complaints_stats**: Useful for getting a quick count without retrieving full complaint details.

Get complaint count statistics
- **get_complaints_with_narrative**: Supports filtering by product, company and state.

Get complaints that include consumer narratives (detailed descriptions)
- **get_recent_complaints**: Useful for tracking recent complaint trends.

Get the most recent consumer complaints
- **search_complaints**: 8M+ complaints against financial companies. Supports filtering by product, company, state, issue, date range and narrative availability. Returns complaint details including product type, company name, issue, state, date received and company response.

Search consumer complaints in the CFPB database


## Installation & Usage

To install and use the **CFPB Complaints** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cfpb-complaints](https://vinkius.com/mcp/cfpb-complaints)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

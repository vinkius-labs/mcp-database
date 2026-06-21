# BOE (Boletín Oficial del Estado) MCP Server

Access the Spanish Official State Gazette (BOE) — search consolidated legislation, daily summaries, and legal analysis directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/boe-boletin-oficial-del-estado)

## Overview
**Category:** knowledge-management
**Tools Count:** 17

## Description
Connect to the **Boletín Oficial del Estado (BOE)** Open Data service to navigate the Spanish legal system through natural conversation. This server provides comprehensive access to official gazettes and updated laws.

### What you can do

- **Consolidated Legislation** — Search for the latest updated versions of Spanish laws and regulations using `search_consolidated_legislation`
- **Daily Summaries** — Retrieve the full index of documents published in the BOE or BORME (Mercantile Registry) for any specific date
- **Legal Analysis** — Access detailed metadata, European Legislation Identifiers (ELI), and relations between different legal norms
- **Full Text Access** — Fetch the complete text of laws or specific blocks (articles/sections) to analyze legal requirements
- **Structural Indexing** — Understand the hierarchy of a law by listing its internal blocks and sections

### How it works

1. Subscribe to this server
2. Enable the connection (Public Open Data access)
3. Start querying Spanish legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly find specific articles or check the latest updates to consolidated codes without manual searching
- **Compliance Officers** — monitor daily publications in the BOE and BORME to ensure regulatory alignment
- **Researchers & Citizens** — explore the Spanish legal framework and historical gazette records through an intuitive AI interface


## Available Tools
- **get_boe_summary**: Get daily summary of the BOE
- **get_borme_summary**: Get daily summary of the BORME
- **get_consolidated_legislation**: ID format: BOE-A-YYYY-NUMBER.

Get consolidated legislation by ID
- **get_legislation_analysis**: Get legal analysis for consolidated legislation
- **get_legislation_block**: g., a specific article).

Get specific block of consolidated legislation
- **get_legislation_eli_metadata**: Get ELI metadata for consolidated legislation
- **get_legislation_metadata**: Get metadata for consolidated legislation
- **get_legislation_text_index**: ) structuring the latest version.

Get text index of consolidated legislation
- **get_legislation_text**: Get full text of consolidated legislation
- **list_consolidation_states**: List auxiliary consolidation states
- **list_departments**: ).

List auxiliary issuing departments
- **list_posterior_relations**: List auxiliary posterior legal relations
- **list_previous_relations**: List auxiliary previous legal relations
- **list_ranks**: ).

List auxiliary legal ranks
- **list_scopes**: List auxiliary scopes
- **list_subjects**: List auxiliary subjects/topics
- **search_consolidated_legislation**: Search consolidated legislation


## Installation & Usage

To install and use the **BOE (Boletín Oficial del Estado)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boe-boletin-oficial-del-estado](https://vinkius.com/mcp/boe-boletin-oficial-del-estado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

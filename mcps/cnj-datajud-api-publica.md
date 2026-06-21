# CNJ (Datajud API Pública) MCP Server

Access the Brazilian National Council of Justice (CNJ) Datajud API to query judicial processes, procedural classes, and court organs across Brazil.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cnj-datajud-api-publica)

## Overview
**Category:** data-management
**Tools Count:** 3

## Description
Connect to the **CNJ Datajud Public API** to perform deep searches across the Brazilian judicial system. This server allows AI agents to retrieve detailed metadata about lawsuits, court movements, and procedural history directly from the official national database.

### What you can do

- **Search by CNJ Number** — Retrieve full details of a specific lawsuit using its unique unformatted numbering and the target court alias.
- **Class & Organ Filtering** — Find processes categorized by their Procedural Class (TPU) and specific Court Organ codes.
- **Advanced Elasticsearch Queries** — Execute complex searches using the full power of Elasticsearch Query DSL to filter by dates, parties, or specific metadata fields.
- **Court Coverage** — Access data from various courts including TRFs, TJs, TST, and more via their respective API aliases.

### How it works

1. Subscribe to this server
2. Enter your CNJ Datajud API Key
3. Start querying the Brazilian judicial database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — Quickly check the status and history of lawsuits without manual portal navigation.
- **Compliance Teams** — Automate background checks and legal risk assessments using official government data.
- **Researchers & Analysts** — Perform bulk queries and advanced data extraction for legal statistics and trends.


## Available Tools
- **search_processes_advanced**: Execute an advanced Elasticsearch query against the Datajud API
- **search_processes_by_class_and_organ**: Search processes by Procedural Class and Court Organ
- **search_process_by_number**: g., api_publica_trf1, api_publica_tjsp).

Search for a specific judicial process by its CNJ number


## Installation & Usage

To install and use the **CNJ (Datajud API Pública)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnj-datajud-api-publica](https://vinkius.com/mcp/cnj-datajud-api-publica)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

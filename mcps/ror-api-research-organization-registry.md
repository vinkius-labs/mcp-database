# ROR API (Research Organization Registry) MCP Server

Access the global registry of research organizations to search, identify, and retrieve detailed metadata for academic and research institutions.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ror-api-research-organization-registry)

## Overview
**Category:** data-management
**Tools Count:** 3

## Description
Connect to the **Research Organization Registry (ROR)**, the community-led registry of open identifiers for research organizations worldwide. This MCP server allows your AI agent to interact with over 100,000 organization records to ensure data accuracy in scholarly communications.

### What you can do

- **Search Organizations** — Use keyword searches, advanced Elasticsearch syntax, or affiliation strings to find specific research entities via `list_organizations`.
- **Detailed Metadata** — Fetch complete records including ROR IDs, website domains, location data, and external identifiers (GRID, ISNI, Crossref) using `get_organization`.
- **Affiliation Matching** — Resolve unstructured affiliation strings from research papers to official ROR identifiers for better data cleaning.
- **System Health** — Monitor the operational status of the ROR API via `get_heartbeat` checks.

### How it works

1. Subscribe to this server
2. (Optional) Enter your ROR Client ID for identified traffic
3. Start querying research institutions directly from your AI assistant

### Who is this for?

- **Data Scientists & Librarians** — Automate the cleaning of institutional affiliation data and map internal IDs to global standards.
- **Academic Developers** — Integrate institutional metadata into research management systems or repositories.
- **Policy Analysts** — Aggregate research output data by accurately identifying parent and child organizations.


## Available Tools
- **get_organization**: Accepts full URL, domain+ID, or ID only.

Retrieve a single ROR organization record
- **get_heartbeat**: Check if the ROR API is operational
- **list_organizations**: Use query, query_advanced, or affiliation for searching.

Retrieve a list of ROR organizations or search via query


## Installation & Usage

To install and use the **ROR API (Research Organization Registry)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ror-api-research-organization-registry](https://vinkius.com/mcp/ror-api-research-organization-registry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

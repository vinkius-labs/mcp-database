# ROR API (Research Organization Registry) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ror-api-research-organization-registry)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ror-api-research-organization-registry-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ror-api-research-organization-registry-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the global registry of research organizations to search, identify, and retrieve detailed metadata for academic and research institutions.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ROR API (Research Organization Registry)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for research organizations in Brazil with the type 'education'."

**🤖 AI Agent:**
> I'll search the ROR registry for you. Using `list_organizations` with the filter `types:education,locations.geonames_details.country_code:BR`, I found several institutions including 'Universidade de São Paulo' (ROR: 0369vth32).

---

**👤 You:**
> "Get the full record for ROR ID 015w2mp89."

**🤖 AI Agent:**
> Fetching details for `015w2mp89`... This record corresponds to 'University of Cambridge'. It is an active education institution located in the United Kingdom, with external IDs including GRID: grid.5335.0.

---

**👤 You:**
> "Check if the ROR API is currently online."

**🤖 AI Agent:**
> I'll check the system status using `get_heartbeat`. The ROR API responded with 'OK', so the service is fully operational.


## Installation & Usage

To install and use the **ROR API (Research Organization Registry)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ror-api-research-organization-registry](https://vinkius.com/mcp/ror-api-research-organization-registry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

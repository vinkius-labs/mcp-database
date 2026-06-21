# OpenSanctions MCP Server

Screen persons and companies against global sanctions lists and PEP databases for KYC/AML compliance.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opensanctions)

## Overview
**Category:** security-compliance
**Tools Count:** 8

## Description
Connect to **OpenSanctions** and access the world's largest open sanctions and PEP screening database through natural conversation — no API key needed for non-commercial use.

### What you can do

- **Entity Search** — Search for sanctioned persons, companies and vessels by name
- **Sanctions Screening** — Screen names against global sanctions lists (OFAC, EU, UN, UK HMT)
- **PEP Screening** — Screen persons against Politically Exposed Persons databases
- **Entity Details** — Get full entity info including aliases, dates of birth, nationalities and addresses
- **Vessel Search** — Search sanctioned vessels by name or IMO number
- **Dataset Browser** — Browse all available sanctions datasets worldwide

### How it works

1. Subscribe to this server
2. No API key needed for non-commercial use
3. Start screening against sanctions lists from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers** — screen clients and partners against global sanctions lists
- **Financial Institutions** — perform KYC/AML checks on customers and transactions
- **Researchers** — explore sanctions data, PEP databases and entity relationships


## Available Tools
- **get_datasets**: Returns dataset names, descriptions, publisher info and entity counts.

Get list of all sanctions datasets available
- **get_entity**: Returns full entity details including names, aliases, dates of birth, nationalities, addresses, sanctions details, related entities and source datasets.

Get detailed info for a specific entity by ID
- **match_pep**: Returns match scores, matched entities, political positions and source datasets. Useful for KYC/AML compliance checks.

Screen a name against Politically Exposed Persons (PEP) lists
- **match_sanctions**: Uses fuzzy matching to find potential matches. Returns match scores, matched entities and sanction details. Use threshold parameter (0.0-1.0) to adjust sensitivity. Default 0.85.

Screen a name against global sanctions lists
- **search_company**: Returns company names, registration numbers, jurisdictions, addresses and sanctions status.

Search for companies in the sanctions database
- **search_entities**: Supports free-text search with fuzzy matching. Returns entity names, types (Person, Company, Vessel), countries and dataset sources. Use schema parameter to filter by entity type (Person, Company, Vessel, etc.).

Search sanctions and PEP entities by name
- **search_person**: Returns person names, aliases, dates of birth, nationalities, countries and sanctions status.

Search for persons in the sanctions database
- **search_vessel**: Returns vessel names, IMO numbers, flags, owners and sanctions status.

Search for vessels (ships) in the sanctions database


## Installation & Usage

To install and use the **OpenSanctions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensanctions](https://vinkius.com/mcp/opensanctions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

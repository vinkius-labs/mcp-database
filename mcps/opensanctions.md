# OpenSanctions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensanctions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opensanctions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opensanctions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Screen persons and companies against global sanctions lists and PEP databases for KYC/AML compliance.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSanctions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Screen 'Vladimir Putin' against sanctions lists."

**🤖 AI Agent:**
> Found multiple matches for Vladimir Putin in OFAC, EU and UK sanctions lists. Includes aliases, dates of birth, nationalities and sanctions details.

---

**👤 You:**
> "Search for companies sanctioned in Russia."

**🤖 AI Agent:**
> Found 50+ sanctioned companies with Russian connections. Includes Gazprom, Rosneft, Sberbank and many others across OFAC, EU and UK sanctions lists.

---

**👤 You:**
> "What sanctions datasets are available?"

**🤖 AI Agent:**
> Available datasets: US OFAC (9,000+ entities), EU Consolidated List (6,000+), UN Security Council (700+), UK HMT (3,000+), and 40+ more global sanctions regimes.


## Installation & Usage

To install and use the **OpenSanctions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensanctions](https://vinkius.com/mcp/opensanctions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

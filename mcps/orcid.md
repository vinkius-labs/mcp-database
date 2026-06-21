# ORCID MCP Server

Access and manage ORCID researcher records — search the registry, fetch biographical data, and manage works or affiliations directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/orcid)

## Overview
**Category:** knowledge-management
**Tools Count:** 13

## Description
Connect to the **ORCID** (Open Researcher and Contributor ID) registry to identify and connect researchers with their professional activities across disciplines and borders.

### What you can do

- **Record Retrieval** — Fetch full summary views or specific biographical sections of any researcher using their 16-digit ORCID iD.
- **Activity Tracking** — Query summaries of all activities including works, funding, and institutional affiliations.
- **Registry Search** — Search the global ORCID database using Solr syntax to find researchers by name, email, or keywords.
- **Item Management** — Deep dive into specific works or funding items using unique put-codes to retrieve full metadata.
- **Member API Features** — For authorized users, create, update, or delete items within sections to keep researcher profiles synchronized.

### How it works

1. Subscribe to this server
2. Enter your ORCID Access Token (Public or Member API)
3. Start querying academic records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Academic Researchers** — quickly verify profile data and manage your own publication list without manual entry
- **University Administrators** — automate the retrieval of faculty activities and affiliations for reporting
- **Data Scientists** — search and analyze researcher metadata for bibliometric studies and mapping scientific networks


## Available Tools
- **create_item**: Requires Member API access and appropriate scopes.

Add a new item to a section (Member API only)
- **csv_search**: Search the ORCID registry and return CSV format
- **delete_item**: Requires Member API access.

Delete an item from a section (Member API only)
- **expanded_search**: Search the ORCID registry and return expanded metadata
- **get_activities**: Get summary of all activities for an ORCID record
- **get_item**: Get a specific item from a section using its put-code
- **get_person**: Get biographical section of an ORCID record
- **get_record**: Get summary view of the full ORCID record
- **get_section**: Get summary of a specific section
- **get_summary**: Requires Member API access.

Get validated and self-asserted summary (Member API only)
- **register_webhook**: Requires Premium Member API.

Register a webhook callback URL for an ORCID record (Premium only)
- **search**: Supports fields like given-names, family-name, email, orcid, etc.

Search the ORCID registry using Solr 3.6 syntax
- **update_item**: Requires Member API access.

Update an existing item in a section (Member API only)


## Installation & Usage

To install and use the **ORCID** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orcid](https://vinkius.com/mcp/orcid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# ORCID (Researcher IDs) MCP Server

Connect to the ORCID registry to search for researchers, fetch biographical data, and manage research activities like works and funding.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/orcid-researcher-ids)

## Overview
**Category:** knowledge-management
**Tools Count:** 14

## Description
Connect the **ORCID** registry to your AI agent to seamlessly navigate the global ecosystem of researcher identifiers and scholarly records.

### What you can do

- **Registry Search** — Perform standard or expanded Solr searches to find researchers by name, institution, or keywords using `search` and `expanded_search`.
- **Profile Summaries** — Retrieve complete researcher records, including biographical details and activity summaries, via `get_record` and `get_activities`.
- **Works & Funding** — Inspect specific research outputs and funding history using `get_works` or drill down into specific items with `get_section_item`.
- **Trust Markers** — Access validated trust markers for records using `get_summary` (requires Member API).
- **Record Management** — Add or update items in an ORCID record directly through the agent using `add_item` and `update_item` (requires Member API).

### How it works

1. Subscribe to this server
2. Enter your ORCID Access Token (Public or Member API)
3. Start querying researcher data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Academic Researchers** — quickly find collaborators and verify publication records without manual searching
- **Librarians & Data Managers** — automate the retrieval of institutional research outputs and metadata
- **Grant Officers** — verify researcher credentials and funding history directly within your workflow


## Available Tools
- **add_item**: Requires Member API access token with /activities/update or /person/update scope.

Add a new item to an ORCID record (Member API only)
- **csv_search**: Search the ORCID registry and return CSV data
- **delete_item**: Requires Member API access token.

Delete an item from an ORCID record (Member API only)
- **expanded_search**: Search the ORCID registry (Expanded)
- **get_activities**: Get summary of all activities for an ORCID record
- **get_person**: Get biographical section of an ORCID record
- **get_record**: Get full summary of an ORCID record
- **get_section_item**: Get full details for a specific item in an ORCID record
- **get_summary**: Requires Member API access token.

Get validated trust markers (Member API only)
- **get_works**: Get summary of research works for an ORCID record
- **register_webhook**: Requires /webhook scope.

Register a webhook for an ORCID record (Premium Member API only)
- **search**: Search the ORCID registry (Standard)
- **unregister_webhook**: Unregister a webhook for an ORCID record (Premium Member API only)
- **update_item**: Requires Member API access token.

Update an existing item in an ORCID record (Member API only)


## Installation & Usage

To install and use the **ORCID (Researcher IDs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orcid-researcher-ids](https://vinkius.com/mcp/orcid-researcher-ids)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

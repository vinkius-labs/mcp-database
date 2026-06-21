# DataCite REST MCP Server

Manage and query DOIs (Digital Object Identifiers) via DataCite — retrieve metadata, list activities, and manage research records directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datacite-rest)

## Overview
**Category:** document-management
**Tools Count:** 12

## Description
Connect to the **DataCite REST API** to interact with the global infrastructure for research data. This MCP server allows your AI agent to search, retrieve, and manage DOIs and their associated metadata.

### What you can do

- **DOI Management** — Create, update, and delete DOI records (Draft state) with full JSON:API support.
- **Metadata Retrieval** — Fetch detailed metadata for any DOI, including affiliations and publisher info.
- **Search & Discovery** — List DOIs with advanced filtering by client, provider, prefix, or resource type.
- **Provenance & Events** — Track metadata changes through activities and discover citations or usage via events.
- **Infrastructure Overview** — List repository accounts (clients), providers, and prefixes within the DataCite network.

### How it works

1. Subscribe to this server
2. Enter your DataCite credentials (Username and Password)
3. Start managing research identifiers from Claude, Cursor, or any MCP-compatible client

No more manual searching through web portals to find research citations or metadata. Your AI acts as a dedicated research data manager.

### Who is this for?

- **Researchers & Academics** — instantly retrieve metadata and citations for specific datasets or publications
- **Data Librarians** — manage DOI records and verify metadata provenance directly from their workflow
- **Developers** — integrate scholarly metadata and DOI registration into automated research pipelines


## Available Tools
- **create_doi**: Requires Member API authentication (Repository account). Payload must follow JSON:API format.

Create a new DOI record
- **delete_doi**: Only DOIs in Draft state can be deleted. Requires Member API authentication.

Delete a DOI (Draft state only)
- **get_doi**: Retrieve metadata for a specific DOI
- **get_heartbeat**: Check API status
- **list_activities**: Retrieve metadata provenance (history of changes)
- **list_clients**: List DataCite Repository accounts
- **list_dois**: Retrieve a list of DOIs
- **list_events**: Retrieve links between DOIs and other resources (citations, usage)
- **list_prefixes**: List DOI prefixes
- **list_providers**: List DataCite Members and Consortium Organizations
- **list_reports**: List usage reports
- **update_doi**: Requires Member API authentication. Only included attributes will be updated.

Update an existing DOI record


## Installation & Usage

To install and use the **DataCite REST** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datacite-rest](https://vinkius.com/mcp/datacite-rest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

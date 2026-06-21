# DataCite REST MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datacite-rest)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datacite-rest-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datacite-rest-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage and query DOIs (Digital Object Identifiers) via DataCite — retrieve metadata, list activities, and manage research records directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DataCite REST** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the metadata for DOI 10.14454/qdd3-ps68."

**🤖 AI Agent:**
> I've retrieved the metadata for DOI 10.14454/qdd3-ps68. It refers to 'DataCite Content Negotiation' published by DataCite. Would you like to see the full list of creators or the associated resource type?

---

**👤 You:**
> "Search for DOIs related to 'climate change' from the last year."

**🤖 AI Agent:**
> I found several DOIs matching 'climate change'. Notable records include datasets from various repositories. I can filter these by resource type or provider if you'd like to narrow it down.

---

**👤 You:**
> "List the events or citations associated with DOI 10.14454/qdd3-ps68."

**🤖 AI Agent:**
> Fetching events... I've found the links between this DOI and other resources, including citations and usage metrics recorded in the DataCite Event Data system.


## Installation & Usage

To install and use the **DataCite REST** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datacite-rest](https://vinkius.com/mcp/datacite-rest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

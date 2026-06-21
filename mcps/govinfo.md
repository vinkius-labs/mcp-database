# GovInfo MCP Server

Search and retrieve official US Government documents and publications via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/govinfo)

## Overview
**Category:** the-unthinkable
**Tools Count:** 8

## Description
Connect to the official **GovInfo** API and empower your AI agent with direct access to official publications from all three branches of the US Federal Government. Query congressional bills, federal regulations, court opinions, and presidential documents using natural language without navigating complex government databases.

### What you can do

- **Document Discovery** — List available document collections and find specific packages based on date ranges or collection codes (e.g., BILLS, FR, CHRG)
- **Deep Search** — Perform complex searches across the entire GovInfo database to find relevant legislative or regulatory documents
- **Daily Updates** — Retrieve a list of all documents officially published on a specific date
- **Metadata Extraction** — Get detailed summary metadata for specific packages or their sub-documents (granules)
- **Contextual Relationships** — Discover related documents to understand the legislative or regulatory history of a specific bill or rule

### How it works

1. Subscribe to this server
2. Enter your free API key from api.data.gov
3. Start querying government documents from Claude, Cursor, or any MCP-compatible client

Your AI agent acts as a dedicated research assistant, capable of instantly locating the exact federal document you need for compliance, research, or legal analysis.

### Who is this for?

- **Legal & Compliance Teams** — quickly locate specific Federal Register notices or track the progress of congressional bills
- **Researchers & Journalists** — retrieve official court opinions and presidential documents directly into your workspace
- **Policy Analysts** — monitor daily government publications and discover related documents for comprehensive policy tracking


## Available Tools
- **get_collection**: Get packages within a collection by date range
- **get_granule_summary**: Get summary metadata for a specific granule
- **get_package_summary**: Get summary metadata for a specific package
- **get_published**: Get documents published on a specific date
- **get_related_documents**: Get documents related to a specific package
- **list_collections**: List available document collections
- **list_package_granules**: List granules (sub-documents) for a package
- **search_documents**: Search documents via the GovInfo Search API


## Installation & Usage

To install and use the **GovInfo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/govinfo](https://vinkius.com/mcp/govinfo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

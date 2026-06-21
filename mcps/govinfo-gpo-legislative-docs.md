# GovInfo (GPO Legislative Docs) MCP Server

Access official US government documents, legislative bills, and federal registers directly from the GPO.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)

## Overview
**Category:** document-management
**Tools Count:** 6

## Description
Connect your AI agent to the **GovInfo** API by the U.S. Government Publishing Office (GPO) to research and retrieve official federal documents through natural conversation.

### What you can do

- **Explore Collections** — List all available document categories like Congressional Bills, the Federal Register, and Presidential Papers
- **Advanced Search** — Use Lucene syntax to perform complex queries across the entire GPO database for specific keywords or topics
- **Document Retrieval** — Fetch detailed metadata, summaries, and historical context for specific legislative packages
- **Content Access** — Retrieve document content in multiple formats including PDF, XML, and MODS for deep analysis
- **Date-based Filtering** — Track legislative changes and new publications by listing packages within specific timeframes

### How it works

1. Subscribe to this server
2. Enter your GovInfo (Data.gov) API Key
3. Start querying official government data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly find specific bill versions, federal regulations, or court opinions without manual portal navigation
- **Researchers & Journalists** — track government activity, historical records, and policy changes using automated queries
- **Policy Analysts** — monitor legislative progress and federal notices in real-time to stay ahead of regulatory shifts


## Available Tools
- **get_collection_details**: Get metadata for a specific GovInfo collection
- **get_package_content**: Note: Binary formats like pdf or zip will be returned as raw text/binary strings.

Download or retrieve GovInfo package content
- **get_package_summary**: Get detailed metadata for a specific GovInfo package
- **list_collections**: g., Congressional Bills, Federal Register).

List all available GovInfo document collections
- **list_packages**: List packages within a GovInfo collection by date
- **search_govinfo**: Search GovInfo collections


## Installation & Usage

To install and use the **GovInfo (GPO Legislative Docs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/govinfo-gpo-legislative-docs](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

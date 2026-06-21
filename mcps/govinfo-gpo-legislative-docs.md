# GovInfo (GPO Legislative Docs) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/govinfo-gpo-legislative-docs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/govinfo-gpo-legislative-docs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Access official US government documents, legislative bills, and federal registers directly from the GPO.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GovInfo (GPO Legislative Docs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available GovInfo document collections."

**🤖 AI Agent:**
> I've retrieved the available collections. You can access documents from the Federal Register (FR), Congressional Bills (BILLS), Daily Compilation of Presidential Documents (DCPD), and many others. Which collection would you like to explore?

---

**👤 You:**
> "Search for recent Congressional Bills related to 'artificial intelligence'."

**🤖 AI Agent:**
> Searching the database... I found several recent bills, including 'H.R. 3849' and 'S. 1624'. Would you like me to fetch the summary for one of these specific packages?

---

**👤 You:**
> "Get the summary and metadata for package ID BILLS-117hr3076ih."

**🤖 AI Agent:**
> Here is the summary for H.R. 3076 (Postal Service Reform Act of 2022). It was introduced in the 117th Congress and focuses on the financial stability of the USPS. I have also retrieved the MODS and XML metadata links if you need further details.


## Installation & Usage

To install and use the **GovInfo (GPO Legislative Docs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/govinfo-gpo-legislative-docs](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

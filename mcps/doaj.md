# DOAJ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doaj)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doaj-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doaj-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and manage open access research journals and articles via the Directory of Open Access Journals (DOAJ).

## Description
Connect to the **Directory of Open Access Journals (DOAJ)** to explore millions of open access articles and journals. This server allows researchers to query metadata and publishers to manage their records through natural conversation.

### What you can do

- **Journal Discovery** — Search the DOAJ database for journals using Elasticsearch syntax, including title, ISSN, and subject filters.
- **Article Search** — Find specific research papers and articles across thousands of open access publications.
- **Metadata Retrieval** — Fetch complete metadata for specific articles using their unique DOAJ IDs.
- **Publisher Management** — Create, update, or delete article records directly from your AI agent (requires API key).
- **Bulk Operations** — Upload high-volume batches of articles asynchronously for efficient catalog management.
- **Journal Applications** — Submit update requests for existing journals to keep directory information current.

### How it works

1. Subscribe to this server
2. (Optional) Enter your DOAJ API Key for publisher features
3. Start searching or managing academic content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find open access sources and metadata without manual database browsing
- **Publishers** — manage article listings and journal updates directly from a command-line or AI interface
- **Librarians & Data Scientists** — automate the retrieval of scholarly metadata for analysis or cataloging


## Available Tools
- **bulk_create_articles**: Requires publisher API key. Keep batch sizes around 600KB.

Bulk upload articles to DOAJ
- **create_application**: Include the journal ID in admin.current_journal.

Submit an update request (application) for an existing journal
- **create_article**: Requires publisher API key. Creating an article with an existing DOI or full-text URL will overwrite the existing record.

Create a new article in DOAJ
- **delete_article**: Requires publisher API key.

Delete an article from DOAJ
- **get_article**: Retrieve a specific DOAJ article by ID
- **search_articles**: Supports fielded search (e.g., bibjson.title:"Quantum").

Search DOAJ articles using Elasticsearch query string syntax
- **search_journals**: Supports fielded search (e.g., bibjson.title:"Journal of Science").

Search DOAJ journals using Elasticsearch query string syntax
- **update_article**: Requires publisher API key.

Update an existing DOAJ article


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOAJ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for open access journals about 'Quantum Computing' in DOAJ."

**🤖 AI Agent:**
> I found several journals. Notable ones include 'Quantum Information Processing' and 'Nature Communications' (Open Access articles). Would you like to see the full list or filter by a specific publisher?

---

**👤 You:**
> "Find articles with 'CRISPR' in the title published in 2023."

**🤖 AI Agent:**
> Searching articles... I found 12 articles matching 'CRISPR' from 2023. One example is 'CRISPR-Cas9 Gene Editing in Agriculture' (ID: 98765). Should I retrieve the full metadata for this article?

---

**👤 You:**
> "Get the full metadata for DOAJ article ID '12039402123'."

**🤖 AI Agent:**
> Retrieving details for article 12039402123... The article is titled 'Sustainable Energy Systems', published in the 'Journal of Renewable Power'. It includes full-text links, author list, and abstract. Would you like the abstract text?


## Installation & Usage

To install and use the **DOAJ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doaj](https://vinkius.com/mcp/doaj)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

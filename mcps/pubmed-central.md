# PubMed Central MCP Server

Search and retrieve full-text biomedical and life sciences literature from PubMed Central (PMC).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pubmed-central)

## Overview
**Category:** knowledge-management
**Tools Count:** 7

## Description
Connect your AI agent to **PubMed Central (PMC)**, the world's premier digital archive of biomedical and life sciences journal literature. This server enables deep exploration of millions of open-access articles directly through natural conversation.

### What you can do

- **Advanced Search** — Use `search_articles` to find PMCIDs matching complex queries, including authors, dates, and specific filters.
- **Full-Text Retrieval** — Access complete article content in BioC XML or JSON formats using `get_bioc_article` for deep analysis.
- **Citation Analysis** — Track the scientific impact of research by finding articles that cite a specific PMID with `get_citing_articles`.
- **Identifier Mapping** — Seamlessly convert between PMCIDs, PMIDs, and DOIs using `convert_ids` to ensure data consistency.
- **Metadata Harvesting** — Retrieve document summaries, license information, and file locations for Open Access records via `get_article_summary` and `get_oa_record`.

### How it works

1. Subscribe to this server
2. Provide your NCBI Tool Name and Email (and an optional API Key for higher rate limits)
3. Start querying the global repository of medical knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — Instantly find relevant literature and extract data from full-text papers without manual downloading.
- **Healthcare Professionals** — Quickly verify medical facts and access the latest clinical studies directly from your workspace.
- **Data Scientists** — Automate the collection of biomedical datasets and citation networks for large-scale analysis.


## Available Tools
- **get_bioc_article**: Retrieve full-text articles via the BioC API
- **get_citing_articles**: Find PMC articles that cite a specific PubMed ID
- **convert_ids**: Convert between article identifiers (PMCID, PMID, DOI)
- **get_oa_record**: Find citation data, license info, and file locations for OA articles
- **oai_pmh_request**: Harvest metadata via the PMC OAI-PMH Service
- **search_articles**: Search for articles in PubMed Central
- **get_article_summary**: Get metadata summaries for PMC articles


## Installation & Usage

To install and use the **PubMed Central** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubmed-central](https://vinkius.com/mcp/pubmed-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

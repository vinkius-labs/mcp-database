# PubMed Central MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pubmed-central)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pubmed-central-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pubmed-central-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and retrieve full-text biomedical and life sciences literature from PubMed Central (PMC).

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PubMed Central** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search PubMed Central for recent articles about 'CRISPR gene editing' published in 2023."

**🤖 AI Agent:**
> I found several articles. Notable ones include PMC1012345 ('Advances in CRISPR...') and PMC1023456. Would you like a summary of the most relevant one?

---

**👤 You:**
> "Get the full-text content of article PMC7840891 in JSON format."

**🤖 AI Agent:**
> I've retrieved the BioC JSON for PMC7840891. It contains sections for Introduction, Methods, Results, and Discussion. Which part should I analyze first?

---

**👤 You:**
> "Convert the DOI 10.1038/s41586-020-2012-7 to a PMCID."

**🤖 AI Agent:**
> The DOI 10.1038/s41586-020-2012-7 maps to PMCID: PMC7095063 (and PMID: 32015508).


## Installation & Usage

To install and use the **PubMed Central** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pubmed-central](https://vinkius.com/mcp/pubmed-central)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

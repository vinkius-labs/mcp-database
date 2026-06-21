# Elsevier ScienceDirect MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elsevier-sciencedirect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/elsevier-sciencedirect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/elsevier-sciencedirect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of scientific, technical, and medical research articles and book chapters directly from your AI agent.

## Description
Connect to **Elsevier ScienceDirect** to empower your AI agent with the world's leading source of scientific, technical, and medical research. This MCP server allows for deep exploration of peer-reviewed literature, metadata retrieval, and access rights verification.

### What you can do

- **Search & Discovery** — Use advanced Boolean queries via `search_sciencedirect` to find articles, journals, and books across the entire database.
- **Full-Text & Abstracts** — Retrieve complete article content or concise abstracts using `get_article` with PII, DOI, or Scopus IDs.
- **Metadata & Citations** — Fetch detailed metadata for institutional repositories or citation management using `get_article_metadata`.
- **Journal & Book Insights** — Access specific metadata for serials (ISSN) via `get_serial_title` and non-serials (ISBN) via `get_nonserial_title`.
- **Access Verification** — Check entitlements and hosting permissions using `get_article_entitlement` and `get_hosting_permissions` to ensure compliant content usage.

### How it works

1. Subscribe to this server
2. Enter your Elsevier API Key (and optional Institutional Token)
3. Start querying scientific literature from Claude, Cursor, or any MCP-compatible client

No more manual searching through web portals. Your AI acts as a research assistant capable of fetching precise data from the ScienceDirect ecosystem.

### Who is this for?

- **Researchers & Academics** — instantly retrieve paper abstracts and full texts without leaving the research environment
- **Data Scientists** — automate the collection of metadata and subject classifications for literature reviews
- **Librarians & Repository Managers** — verify hosting permissions and entitlements for institutional compliance


## Available Tools
- **get_article_entitlement**: Check user access rights for an article
- **get_article_metadata**: Retrieve article metadata lookups
- **get_article**: Retrieve full-text or abstract of an article
- **get_hosting_permissions**: Retrieve embargo and hosting information
- **get_nonserial_title**: Retrieve metadata for books by ISBN
- **get_object**: Retrieve multimedia or attachments for an article
- **get_serial_title**: Retrieve metadata for journals by ISSN
- **get_subject_classifications**: Retrieve subject categories
- **search_sciencedirect**: Search full-text content on ScienceDirect


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elsevier ScienceDirect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search ScienceDirect for recent articles about CRISPR in Title/Abstract/Keywords."

**🤖 AI Agent:**
> I've found several recent articles on CRISPR. The top results include 'CRISPR-Cas9 Gene Editing in Human Cells' and 'Advances in CRISPR Technology'. Would you like the abstract for any of these?

---

**👤 You:**
> "Get the full text for the article with DOI 10.1016/j.cell.2023.01.001."

**🤖 AI Agent:**
> Retrieving full content for DOI 10.1016/j.cell.2023.01.001... I have successfully fetched the article. It covers new insights into cellular signaling pathways. How would you like me to summarize it?

---

**👤 You:**
> "Check the hosting permissions for PII S0022-2836(21)00123-4."

**🤖 AI Agent:**
> Checking hosting permissions for PII S0022-2836(21)00123-4... This article has an active embargo period ending on 2024-12-01. After this date, it can be hosted in institutional repositories.


## Installation & Usage

To install and use the **Elsevier ScienceDirect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elsevier-sciencedirect](https://vinkius.com/mcp/elsevier-sciencedirect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

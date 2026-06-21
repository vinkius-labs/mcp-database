# CrossRef MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crossref)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crossref-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crossref-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 140M+ scholarly works across all scientific disciplines — with DOI resolution, citation counts, author lookup, and full bibliographic metadata from the world's largest DOI registry.

## Description
Give your AI agent direct access to the **world's largest registry of scholarly metadata** — 140M+ records spanning every DOI ever assigned across all scientific publishers.

### What you can do

- **Universal Search** — Find any published work across journals, books, conference papers, datasets, and dissertations using free-text queries
- **DOI Resolution** — Instant metadata lookup for any DOI with title, complete author list, journal, year, type, and citation count
- **Author Discovery** — Search for all publications by a specific researcher name across all major publishers simultaneously

### How it works

1. Subscribe to this server
2. Start resolving DOIs and searching scholarly works immediately — no API key required

### Who is this for?

- **Academic Researchers** — resolve DOIs, verify citations, and build comprehensive bibliographies without leaving their AI assistant
- **Science Writers** — instantly retrieve publication details to verify facts and cite sources accurately
- **Data Analysts** — explore the scholarly landscape with citation metrics and publisher data for bibliometric analysis


## Available Tools
- **get_crossref_doi**: g. 10.1038/nature12373) and get complete metadata: title, all authors, journal, year, type, citation count, and abstract.

Look up any scholarly work by its DOI
- **search_crossref_author**: Returns their publications sorted by relevance with citation counts.

Find publications by a specific author
- **search_crossref**: Every result includes DOI, citation count, and full bibliographic data. The world's largest DOI registry.

Search 140M+ scholarly works across all scientific disciplines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CrossRef** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up the paper with DOI 10.1038/nature12373 and show me all its details."

**🤖 AI Agent:**
> Found: 'Sequence-specific antimicrobials using efficiently delivered RNA-guided nucleases' by David Bikard et al. Published in Nature Biotechnology (2014). Type: journal-article. Cited 682 times. This is a pioneering paper on using CRISPR-Cas9 for targeted antimicrobial applications. DOI resolves to the publisher page for full-text access.

---

**👤 You:**
> "Find all publications by Jennifer Doudna related to gene editing."

**🤖 AI Agent:**
> Found 10 works by Jennifer Doudna. Top results include her landmark 2012 Science paper 'A Programmable Dual-RNA-Guided DNA Endonuclease in Adaptive Bacterial Immunity' (cited 15,000+ times), follow-up work on CRISPR applications in Nature, and reviews in Cell. Each entry includes DOI, journal, year, and full citation count.

---

**👤 You:**
> "Search CrossRef for the latest research on quantum computing error correction."

**🤖 AI Agent:**
> Found 10 relevant works. Highlights: 'Suppressing quantum errors by scaling a surface code logical qubit' in Nature (2023) — cited 320 times. Also found recent work from Google Quantum AI and IBM Research on topological error correction codes. All results include DOI, full author lists, and citation metrics.


## Installation & Usage

To install and use the **CrossRef** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crossref](https://vinkius.com/mcp/crossref)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

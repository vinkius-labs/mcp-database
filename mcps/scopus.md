# Scopus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scopus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scopus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scopus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest abstract and citation database. Search for research papers, authors, and institutional profiles directly.

## Description
Connect your **Scopus** API credentials to any AI agent and unlock the power of Elsevier's massive research database through natural conversation.

### What you can do

- **Advanced Search** — Query Scopus abstracts and metadata using Boolean syntax and field codes like TITLE-ABS-KEY() or PUBYEAR
- **Author & Institution Profiles** — Retrieve detailed profiles, including H-index, affiliation history, and publication lists
- **Citation Metrics** — Get comprehensive citation overviews, counts, and summaries by year for any document via DOI or Scopus ID
- **Journal Insights** — Access metadata for serials including CiteScore, SJR, and SNIP metrics to evaluate publication impact
- **PlumX Metrics** — Inspect social media mentions, usage, and altmetrics to understand the broader reach of scientific work

### How it works

1. Subscribe to this server
2. Enter your Scopus API Key (and optional Institutional Token)
3. Start conducting literature reviews and bibliometric analysis from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — quickly find relevant literature and track citation trends without manual database exports
- **Data Scientists** — integrate high-quality metadata and metrics into research workflows and knowledge graphs
- **University Administrators** — audit institutional output and author profiles with ease


## Available Tools
- **get_abstract**: Get detailed metadata for a specific document
- **get_affiliation**: Get detailed profile for an institution
- **get_author**: Get detailed profile for a specific author
- **get_citation_count**: Get abstract citation count
- **get_citation_overview**: Get citation counts and summaries by year
- **get_plumx_metrics**: Get Altmetrics for Scopus documents
- **get_serial_title**: Get metadata about journals (metrics like CiteScore, SJR, SNIP)
- **search_affiliation**: Search Scopus institutional profiles
- **search_author**: Search Scopus author profiles
- **search_scopus**: Search Scopus abstracts and metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scopus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Scopus for papers about 'Large Language Models' published in 2024."

**🤖 AI Agent:**
> I found several high-impact papers. The top results include 'A Survey of Large Language Models' and 'Efficient Training of LLMs'. Would you like me to fetch the abstract for any of these?

---

**👤 You:**
> "Get the citation overview for DOI 10.1016/j.future.2023.01.001."

**🤖 AI Agent:**
> This document has been cited 45 times since its publication. In 2023 it received 12 citations, and so far in 2024, it has 33. It shows a strong upward trend in the field of cloud computing.

---

**👤 You:**
> "Find the profile and H-index for author ID 7004212771."

**🤖 AI Agent:**
> Author ID 7004212771 corresponds to Dr. Jane Smith. She has an H-index of 52, with 142 total documents and over 8,500 citations. Her primary affiliation is Stanford University.


## Installation & Usage

To install and use the **Scopus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scopus](https://vinkius.com/mcp/scopus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

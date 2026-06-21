# Unpaywall (Open Access Papers) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unpaywall-open-access-papers)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unpaywall-open-access-papers-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unpaywall-open-access-papers-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of open-access scholarly articles. Check OA status and retrieve full-text PDF links using DOIs.

## Description
Connect to the **Unpaywall** database to instantly find legal, open-access versions of scholarly papers. This server allows your AI agent to bypass paywalls by locating freely available PDFs and repository versions of research articles using their Digital Object Identifier (DOI).

### What you can do

- **OA Status Verification** — Instantly check if a specific scholarly article is available for free under an Open Access license.
- **PDF Retrieval** — Get direct links to legal, full-text PDF versions of research papers hosted on publisher sites or institutional repositories.
- **Metadata Inspection** — Retrieve information about the type of Open Access (gold, green, bronze, etc.) and the hosting source.
- **Research Automation** — Streamline literature reviews by letting your agent automatically find accessible versions of cited works.

### How it works

1. Subscribe to this server
2. Enter your email address (required by Unpaywall's API policy)
3. Start searching for open-access papers in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find full-text versions of papers without navigating multiple library portals
- **Students** — access required reading materials that are legally available for free
- **Data Scientists** — automate the collection of open-access research data and papers for analysis


## Available Tools
- **get_article_oa_status**: Retrieve Open Access status and locations for a specific DOI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unpaywall (Open Access Papers)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the Open Access status for DOI 10.1038/nature12345."

**🤖 AI Agent:**
> I've checked the Unpaywall database for DOI 10.1038/nature12345. This article is available via Open Access. You can download the full PDF here: [Link].

---

**👤 You:**
> "Find a free version of the paper with DOI 10.1126/science.1234567."

**🤖 AI Agent:**
> Searching... I found a legal, open-access version of this paper hosted on a university repository. Here is the link to the full text.

---

**👤 You:**
> "Is the article 10.1016/j.cell.2021.01.001 behind a paywall?"

**🤖 AI Agent:**
> According to Unpaywall, this specific DOI is currently not available as a free Open Access version. It appears to be behind a publisher paywall.


## Installation & Usage

To install and use the **Unpaywall (Open Access Papers)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unpaywall-open-access-papers](https://vinkius.com/mcp/unpaywall-open-access-papers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

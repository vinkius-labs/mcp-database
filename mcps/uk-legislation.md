# UK Legislation MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-legislation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uk-legislation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uk-legislation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Official UK legislation database — search acts, statutory instruments, and sections via AI.

## Description
Empower your AI agent with the definitive source for UK law through the **UK Legislation** MCP server. This integration provides real-time access to the official database of Public General Acts, Statutory Instruments, and other legislative documents from the UK Parliament and devolved administrations. Your agent can search for legislation by title, year, or subject, retrieve full tables of contents, and extract specific sections or schedules for analysis. Whether you are conducting legal research, verifying regulatory compliance, or exploring constitutional history, your agent acts as a dedicated legal archivist through natural conversation.

### What you can do

- **Legislative Search** — Find acts and instruments by keyword, title, year, or subject area.
- **Content Extraction** — Retrieve the full text or specific sections/schedules of any piece of legislation.
- **Structural Analysis** — Fetch complete tables of contents to understand the hierarchy of complex acts.
- **Recent Updates** — Monitor the most recently published legislative documents to stay informed of new laws.
- **Historical Reference** — Access primary and secondary legislation enacted throughout history by year.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying UK laws from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly verify specific sections of acts and historical amendments.
- **Policy Researchers** — analyze legislative trends and search for laws by subject area.
- **Compliance Officers** — stay updated with recent statutory instruments and regulatory changes.
- **Students & Academics** — access the primary source of UK law for constitutional and legal studies.


## Available Tools
- **get_legislation_by_year**: List UK legislation for a specific year
- **get_table_of_contents**: Get the table of contents for UK legislation
- **get_legislation**: Get specific UK legislation details
- **get_recent_legislation**: Get recently published UK legislation
- **get_schedule**: Get a specific schedule of UK legislation
- **get_section**: Get a specific section of UK legislation
- **search_by_subject**: Search UK legislation by subject
- **search_legislation**: Returns a list of matching acts, statutory instruments, and other legislative documents.

Search for UK legislation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK Legislation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the 'Data Protection Act 2018' in UK legislation."

**🤖 AI Agent:**
> I've searched the database and found the 'Data Protection Act 2018' (ukpga/2018/12). I can retrieve its full table of contents or specific sections for you. Which part would you like to examine?

---

**👤 You:**
> "List all Public General Acts enacted in 2024."

**🤖 AI Agent:**
> Retrieving the list for 2024... I found several acts including the 'Finance Act 2024'. Would you like me to get the details or table of contents for any of these?

---

**👤 You:**
> "What is Section 1 of the Human Rights Act 1998?"

**🤖 AI Agent:**
> Fetching Section 1... This section defines 'The Convention rights' and lists the specific articles of the European Convention on Human Rights that are given effect in the UK. Would you like me to list those articles?


## Installation & Usage

To install and use the **UK Legislation** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-legislation](https://vinkius.com/mcp/uk-legislation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

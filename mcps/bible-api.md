# Bible API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bible-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bible-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bible-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search and retrieve scripture — audit Bible versions and verses via AI.

## Description
Empower your AI agent to orchestrate your entire biblical research workflow with **Bible API**, the authoritative source for global scripture data. By connecting the American Bible Society's API to your agent, you transform complex verse lookups into a natural conversation. Your agent can instantly search for keywords across hundreds of Bible versions, audit chapter contents, and retrieve detailed verse metadata without you ever touching a technical portal. Whether you are conducting theological research or managing daily devotionals, your agent acts as a real-time biblical consultant, ensuring your data is always grounded in official, historically accurate translations.

### What you can do

- **Scripture Auditing** — Search for specific keywords or phrases across multiple Bible versions and retrieve cleaned text metadata.
- **Version Oversight** — List and query hundreds of Bible translations across dozens of languages to maintain a clear view of linguistic nuances.
- **Verse Discovery** — Retrieve specific verses or entire chapters using unique identifiers to assist in theological study.
- **Book Intelligence** — List all books within a specific Bible version to understand the organizational structure of the canon.
- **Metadata Discovery** — Retrieve detailed descriptions and abbreviations for Bible versions to identify the perfect source for your research.

### How it works

1. Subscribe to this server
2. Enter your API.Bible Key
3. Start managing your biblical intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Theologians & Scholars** — monitor scriptural translations and retrieve verse metadata straight from your workflow.
- **Pastors & Educators** — verify chapter contents and audit biblical books without manual searching.
- **Writers & Content Creators** — perform rapid audits of biblical quotes and identify correct translations through natural language.
- **Operations Leads** — automate scripture data querying to orchestrate cross-functional educational teams smoothly.


## Available Tools
- **get_bible_details**: Get metadata for a specific Bible ID
- **get_bible_chapter**: Get the content of a specific chapter
- **get_bible_verse**: Get the text of a specific verse
- **list_bibles**: List all available Bible versions and languages
- **list_bible_books**: List all books in a specific Bible version
- **search_bible_text**: Search for keywords or phrases across a Bible version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bible API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'love' in the English Standard Version (bibleId: de4e12af7f895f10-01) using Bible API."

**🤖 AI Agent:**
> I've retrieved 10 results for 'love' in the specified version. Notable verses include John 3:16 and 1 Corinthians 13:4. Would you like the full text for any of these results?

---

**👤 You:**
> "Show the content of Genesis chapter 1 from the King James Version."

**🤖 AI Agent:**
> I've retrieved the full text of Genesis 1. It details the creation of the heavens and the earth across seven days. I can provide the text broken down by individual verses if you'd like.

---

**👤 You:**
> "List all Bible versions available in 'Portuguese'."

**🤖 AI Agent:**
> I've scanned the catalog for Portuguese versions. There are over 10 versions available, including Almeida Corrigida Fiel and Nova Versão Internacional. I can provide the specific bibleIds for each.


## Installation & Usage

To install and use the **Bible API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bible-api](https://vinkius.com/mcp/bible-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

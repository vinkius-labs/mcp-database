# OpenAlex MCP Server

Automate scholarly research via OpenAlex — search millions of works, authors, and institutions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openalex-alternative)

## Overview
**Category:** the-unthinkable
**Tools Count:** 14

## Description
Connect to **OpenAlex**, the world's most comprehensive open index of the global research system. Empower your AI agent to navigate the vast landscape of scholarly knowledge through natural conversation.

### What you can do

- **Scholarly Works** — Search, filter, and retrieve metadata for millions of articles, books, and datasets using `list_works` and `get_work`.
- **Author Profiles** — Identify researchers, their affiliations, and impact metrics using `list_authors` and `get_author`.
- **Institutional Insights** — Explore universities and research organizations globally with `list_institutions` and `get_institution`.
- **Venues & Sources** — Inspect journals, conferences, and repositories via `list_sources` and `get_source`.
- **Discovery & Taxonomy** — Navigate topics, publishers, and funders to understand the funding and publication landscape using specialized listing tools.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OpenAlex API Key for the 'Polite Pool' (faster limits)
3. Start querying the world's research from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find relevant literature and track citations without leaving your writing environment
- **Data Scientists** — gather bibliometric data and map research trends programmatically
- **Students** — discover authoritative sources and key authors for any field of study


## Available Tools
- **get_author**: Get a single author by their OpenAlex ID
- **get_funder**: Get a single funder by its OpenAlex ID
- **get_institution**: Get a single institution by its OpenAlex ID
- **get_publisher**: Get a single publisher by its OpenAlex ID
- **get_source**: Get a single source by its OpenAlex ID
- **get_topic**: Get a single topic by its OpenAlex ID
- **get_work**: g., W2741809807).

Get a single scholarly work by its OpenAlex ID
- **list_authors**: Always resolve names to IDs here before filtering works.

List, search, or filter authors
- **list_funders**: List, search, or filter funders
- **list_institutions**: List, search, or filter institutions (universities, research orgs)
- **list_publishers**: List, search, or filter publishers
- **list_sources**: List, search, or filter sources (journals, repositories, conferences)
- **list_topics**: List, search, or filter research topics
- **list_works**: Supports search, filter (e.g., author.id:A123, publication_year:>2020), sort, and group_by.

List, search, or filter scholarly works (articles, books, datasets)


## Installation & Usage

To install and use the **OpenAlex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openalex-alternative](https://vinkius.com/mcp/openalex-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

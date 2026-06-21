# arXiv MCP Server

Access millions of scientific papers from arXiv — search by author, category, or keyword and fetch metadata directly from the open-access archive.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arxiv-alternative)

## Overview
**Category:** the-unthinkable
**Tools Count:** 4

## Description
Connect to **arXiv**, the premier open-access archive for millions of scholarly articles in physics, mathematics, computer science, and more. This MCP server allows your AI agent to browse, search, and harvest scientific knowledge directly from the source.

### What you can do

- **Advanced Search** — Query the legacy API for papers using keywords, authors, or specific categories via the `search_articles` tool.
- **Daily Feeds** — Stay updated with the latest submissions using `get_rss_feed` and `get_atom_feed` for specific scientific domains.
- **Metadata Harvesting** — Use the `oai_pmh_request` interface to retrieve structured metadata, identifiers, and record sets for deep research analysis.
- **ID Lookup** — Instantly fetch details for specific papers by providing a list of unique arXiv identifiers.

### How it works

1. Subscribe to this server
2. (Optional) Enter your arXiv credentials if you have specific access requirements
3. Start exploring the world's scientific literature from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — Automate literature reviews and stay current with the latest preprints in your field.
- **Data Scientists** — Harvest metadata for citation analysis or trend mapping in AI and machine learning.
- **Students** — Quickly find relevant sources and paper summaries for study and projects.


## Available Tools
- **get_atom_feed**: Combine multiple categories with a plus sign (+).

Get the daily Atom feed for a specific arXiv category
- **oai_pmh_request**: Returns raw XML.

Make a request to the arXiv OAI-PMH interface
- **get_rss_feed**: Combine multiple categories with a plus sign (+).

Get the daily RSS feed for a specific arXiv category
- **search_articles**: You can also fetch specific papers by providing a comma-separated list of arXiv IDs.

Search arXiv for articles using the legacy Query API


## Installation & Usage

To install and use the **arXiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arxiv-alternative](https://vinkius.com/mcp/arxiv-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# arXiv MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arxiv-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arxiv-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arxiv-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access millions of scientific papers from arXiv — search by author, category, or keyword and fetch metadata directly from the open-access archive.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **arXiv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search arXiv for recent papers about 'Large Language Models' in the computer science category."

**🤖 AI Agent:**
> I've found several recent papers on Large Language Models. Notable titles include 'Attention is All You Need' and 'Language Models are Few-Shot Learners'. Would you like the full metadata for any of these?

---

**👤 You:**
> "Get the daily RSS feed for the 'cs.AI' category to see today's new submissions."

**🤖 AI Agent:**
> Fetching today's updates for Artificial Intelligence... I've retrieved the latest 10 submissions, including papers on neural network optimization and reinforcement learning. Should I summarize the top results?

---

**👤 You:**
> "Use OAI-PMH to list the metadata formats available on arXiv."

**🤖 AI Agent:**
> I've queried the OAI-PMH interface. arXiv supports several metadata formats including 'oai_dc', 'arXiv', and 'arXivRaw'. Which format would you like to use for harvesting records?


## Installation & Usage

To install and use the **arXiv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arxiv-alternative](https://vinkius.com/mcp/arxiv-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

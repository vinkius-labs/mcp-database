# MemoQ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memoq)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/memoq-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/memoq-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage translation assets via MemoQ — query translation memories, search term bases, and manage linguistic entries directly from your AI agent.

## Description
Connect your **MemoQ** server to any AI agent to streamline your localization and translation workflows. This integration allows for deep inspection and management of linguistic assets through natural language.

### What you can do

- **Translation Memories (TM)** — List available TMs, fetch metadata, and perform concordance searches to find how specific phrases were previously translated.
- **Term Bases (TB)** — Search for industry-specific terminology, lookup terms, and ensure consistency across projects.
- **Entry Management** — Create, update, or delete entries in both Translation Memories and Term Bases to keep your linguistic databases up to date.
- **Segment Lookup** — Perform advanced segment lookups with match thresholds and fuzzy match adjustments.
- **Custom Schemes** — Retrieve custom metadata schemes for TMs to understand specific organizational tagging.

### How it works

1. Subscribe to this server
2. Enter your MemoQ Base URL and Access Token
3. Start querying your translation assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Managers** — quickly verify if a term exists in a TB or check TM coverage without opening the MemoQ desktop client.
- **Translators & Reviewers** — perform concordance searches and term lookups directly from their workspace to maintain consistency.
- **Language Engineers** — automate the maintenance of TMs and TBs by updating entries via AI-driven workflows.


## Available Tools
- **create_tb_entry**: Create a new entry in a Termbase
- **create_tm_entry**: Create a new entry in a TM
- **delete_tb_entry**: Delete an entry from a Termbase
- **delete_tm_entry**: Delete an entry from a TM
- **get_tb_entry**: Get a specific entry from a Termbase
- **get_tb**: Get details for a specific Termbase
- **get_tm_custom_meta_scheme**: Get custom meta scheme for a TM
- **get_tm_entry**: Get a specific entry from a TM
- **get_tm**: Get details for a specific Translation Memory
- **list_tbs**: Can be filtered by language.

List Termbases (TBs)
- **list_tms**: Can be filtered by source and target languages.

List Translation Memories (TMs)
- **tb_lookup_terms**: Lookup terms in a Termbase
- **tb_search**: Search for expressions in a Termbase
- **tm_concordance**: Perform a concordance search in a TM
- **tm_lookup_segments**: Lookup segments in a TM
- **update_tb_entry**: Update an existing entry in a Termbase
- **update_tm_entry**: Update an existing entry in a TM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MemoQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Translation Memories available for English to Portuguese."

**🤖 AI Agent:**
> I've found 3 TMs for that language pair: 'General_EN_PT' (GUID: tm_123), 'Legal_Docs' (GUID: tm_456), and 'Technical_Manuals' (GUID: tm_789).

---

**👤 You:**
> "Search for the term 'cloud computing' in the Term Base with GUID tb_999."

**🤖 AI Agent:**
> Searching TB tb_999... I found one entry: 'Computação em nuvem'. It is marked as the preferred term for Portuguese (Brazil).

---

**👤 You:**
> "Perform a concordance search for 'User Interface' in TM tm_123."

**🤖 AI Agent:**
> I found 5 matches in TM tm_123. The most frequent translation is 'Interface do Usuário'. Would you like to see the full segments?


## Installation & Usage

To install and use the **MemoQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memoq](https://vinkius.com/mcp/memoq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

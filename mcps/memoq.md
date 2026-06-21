# MemoQ MCP Server

Manage translation assets via MemoQ — query translation memories, search term bases, and manage linguistic entries directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/memoq)

## Overview
**Category:** collaboration
**Tools Count:** 17

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


## Installation & Usage

To install and use the **MemoQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memoq](https://vinkius.com/mcp/memoq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

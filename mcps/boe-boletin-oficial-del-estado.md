# BOE (Boletín Oficial del Estado) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boe-boletin-oficial-del-estado)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boe-boletin-oficial-del-estado-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boe-boletin-oficial-del-estado-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the Spanish Official State Gazette (BOE) — search consolidated legislation, daily summaries, and legal analysis directly from your AI agent.

## Description
Connect to the **Boletín Oficial del Estado (BOE)** Open Data service to navigate the Spanish legal system through natural conversation. This server provides comprehensive access to official gazettes and updated laws.

### What you can do

- **Consolidated Legislation** — Search for the latest updated versions of Spanish laws and regulations using `search_consolidated_legislation`
- **Daily Summaries** — Retrieve the full index of documents published in the BOE or BORME (Mercantile Registry) for any specific date
- **Legal Analysis** — Access detailed metadata, European Legislation Identifiers (ELI), and relations between different legal norms
- **Full Text Access** — Fetch the complete text of laws or specific blocks (articles/sections) to analyze legal requirements
- **Structural Indexing** — Understand the hierarchy of a law by listing its internal blocks and sections

### How it works

1. Subscribe to this server
2. Enable the connection (Public Open Data access)
3. Start querying Spanish legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly find specific articles or check the latest updates to consolidated codes without manual searching
- **Compliance Officers** — monitor daily publications in the BOE and BORME to ensure regulatory alignment
- **Researchers & Citizens** — explore the Spanish legal framework and historical gazette records through an intuitive AI interface


## Available Tools
- **get_boe_summary**: Get daily summary of the BOE
- **get_borme_summary**: Get daily summary of the BORME
- **get_consolidated_legislation**: ID format: BOE-A-YYYY-NUMBER.

Get consolidated legislation by ID
- **get_legislation_analysis**: Get legal analysis for consolidated legislation
- **get_legislation_block**: g., a specific article).

Get specific block of consolidated legislation
- **get_legislation_eli_metadata**: Get ELI metadata for consolidated legislation
- **get_legislation_metadata**: Get metadata for consolidated legislation
- **get_legislation_text_index**: ) structuring the latest version.

Get text index of consolidated legislation
- **get_legislation_text**: Get full text of consolidated legislation
- **list_consolidation_states**: List auxiliary consolidation states
- **list_departments**: ).

List auxiliary issuing departments
- **list_posterior_relations**: List auxiliary posterior legal relations
- **list_previous_relations**: List auxiliary previous legal relations
- **list_ranks**: ).

List auxiliary legal ranks
- **list_scopes**: List auxiliary scopes
- **list_subjects**: List auxiliary subjects/topics
- **search_consolidated_legislation**: Search consolidated legislation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BOE (Boletín Oficial del Estado)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the summary of documents published in the BOE for January 10th, 2024."

**🤖 AI Agent:**
> I've retrieved the BOE summary for 20240110. It contains 142 documents across sections like 'General Dispositions', 'Authorities and Personnel', and 'Other Dispositions'. Would you like to see the titles in a specific section?

---

**👤 You:**
> "Search for consolidated legislation related to 'Ley de Propiedad Intelectual'."

**🤖 AI Agent:**
> I found the consolidated version of the Intellectual Property Law (BOE-A-1996-8930). It was last updated on March 30, 2023. Would you like me to fetch the full text or the structural index?

---

**👤 You:**
> "Get the legal analysis and relations for law BOE-A-2015-10565."

**🤖 AI Agent:**
> Analyzing BOE-A-2015-10565 (General Tax Law)... This law has 15 previous relations (norms it modifies or repeals) and 42 posterior relations. It covers subjects like 'Tax Administration' and 'Public Finance'. Should I list the specific laws it modifies?


## Installation & Usage

To install and use the **BOE (Boletín Oficial del Estado)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boe-boletin-oficial-del-estado](https://vinkius.com/mcp/boe-boletin-oficial-del-estado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

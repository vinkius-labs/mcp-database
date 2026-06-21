# BCLaws API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bclaws-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bclaws-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bclaws-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access British Columbia laws — audit statutes and regulations via AI.

## Description
Empower your AI agent to orchestrate your entire legal research and legislative auditing workflow with **BCLaws API**, the authoritative source for British Columbia statutes and regulations. By connecting BCLaws to your agent, you transform complex legal lookups into a natural conversation. Your agent can instantly search for specific laws, audit statute details, and retrieve consolidated regulations without you ever touching a manual database. Whether you are conducting legal due diligence or monitoring regulatory changes, your agent acts as a real-time legislative assistant, ensuring your data is always grounded in official, government-verified records.

### What you can do

- **Legal Auditing** — Search for British Columbia statutes and regulations by keyword and retrieve detailed metadata, including official identifiers.
- **Statute Oversight** — Retrieve full details for specific statutes to maintain a clear view of legislative language and history.
- **Regulation Discovery** — Query provincial regulations to understand the legal constraints and requirements for any activity instantly.
- **Act Monitoring** — List all available Acts in the BCLaws database to identify relevant legislative frameworks for your research.
- **Consolidation Intelligence** — Retrieve consolidated statutes and regulations to maintain strict control over current legal versions.

### How it works

1. Subscribe to this server
2. No API Key required (BCLaws is a public and free service)
3. Start managing your legal intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — monitor statutes and retrieve regulatory metadata straight from your workflow.
- **Policy Analysts** — verify legislative changes and audit provincial laws without manual database searches.
- **Researchers** — perform rapid audits of BC regulations and identify key legal markers through natural language.
- **Operations Leads** — automate legal data querying to orchestrate cross-functional compliance teams smoothly.


## Available Tools
- **check_api_status**: Check if the BCLaws API is operational
- **get_bc_regulation**: Get details for a specific British Columbia regulation
- **get_bc_statute**: Get details for a specific British Columbia statute
- **list_bc_acts**: List all available Acts in the BCLaws database
- **list_consolidated_laws**: List consolidated statutes and regulations
- **search_bc_laws**: Search for British Columbia statutes and regulations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCLaws API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for BC laws related to 'Environmental Protection' using BCLaws API."

**🤖 AI Agent:**
> I've initiated the search for environmental protection laws. Notable matches include the Environmental Management Act and associated regulations. Would you like the full identifiers for these records?

---

**👤 You:**
> "Show details for statute with ID 'EBA'."

**🤖 AI Agent:**
> I've retrieved the details for statute ID 'EBA'. It corresponds to the Evidence Act. I can provide the full legislative text or history if you'd like.

---

**👤 You:**
> "List all available Acts in the BC laws database."

**🤖 AI Agent:**
> I've scanned the catalog. There are hundreds of Acts listed, from administrative statutes to specific provincial laws. I can help you filter the list by keyword or identifier.


## Installation & Usage

To install and use the **BCLaws API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bclaws-api](https://vinkius.com/mcp/bclaws-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

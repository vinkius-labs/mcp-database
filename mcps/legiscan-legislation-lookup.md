# LegiScan Legislation Lookup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legiscan-legislation-lookup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/legiscan-legislation-lookup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/legiscan-legislation-lookup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal legislative intelligence — search bills, votes, and state laws via AI.

## Description
Equip your AI agent with real-time legislative intelligence through the **LegiScan** MCP server. This integration provides instant access to the legislative processes of all 50 US states and Congress. Your agent can search for bills by keyword or ID, retrieve detailed bill summaries and progress, and explore voting records. Whether you are tracking specific policy changes, auditing legislative activity, or researching state laws, your agent acts as a dedicated policy analyst through natural conversation.

### What you can do

- **Bill Search** — Find legislative bills across any state or federal jurisdiction by keyword.
- **Status Tracking** — Monitor the current progress and history of specific legislation.
- **Vote Auditing** — Retrieve detailed voting records for specific bills to see how representatives voted.
- **Master List Retrieval** — Access a complete list of all active bills for a specific session and state.

### How it works

1. Subscribe to this server
2. Enter your LegiScan API Key (get it at legiscan.com)
3. Start monitoring legislation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Analysts & Lobbyists** — track bills and policy shifts across multiple states.
- **Legal Researchers** — access the full history and text of state-level legislation.
- **Journalists** — pull reliable legislative data for political reporting.
- **Active Citizens** — monitor the activity of their state representatives.


## Available Tools
- **get_bill_details**: Get details for a specific bill
- **get_state_master_list**: Get the current master list for a state
- **search_bills**: Search for legislative bills


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LegiScan Legislation Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for California bills related to 'clean energy'."

**🤖 AI Agent:**
> Searching the LegiScan database for California... I've found several active bills related to clean energy, including AB-525 regarding offshore wind and SB-100 updates. Would you like to see the current status of a specific bill?

---

**👤 You:**
> "What is the progress of bill 'NY-S01234'?"

**🤖 AI Agent:**
> Retrieving details for NY-S01234... This bill has passed the Senate and is currently in the Assembly committee. The last action was a favorable report on June 5th. Would you like to see the voting records?

---

**👤 You:**
> "List all federal bills related to 'artificial intelligence'."

**🤖 AI Agent:**
> I've scanned the federal legislative database. There are currently 12 active bills related to AI, including the 'AI Disclosure Act' and the 'Algorithmic Accountability Act'. I can provide summaries for each of them.


## Installation & Usage

To install and use the **LegiScan Legislation Lookup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legiscan-legislation-lookup](https://vinkius.com/mcp/legiscan-legislation-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

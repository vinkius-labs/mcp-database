# Aracaju MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aracaju)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aracaju-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aracaju-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Aracaju's transparency data—revenues, expenses, bids, contracts, and payroll—directly from your AI agent.

## Description
Connect to the **Aracaju Transparency Portal** to audit and analyze public data from the capital of Sergipe, Brazil. This server allows any AI agent to query municipal financial records and administrative data in real-time.

### What you can do

- **Revenues & Income** — List and analyze municipality revenues by fiscal year and month to track tax collection and transfers.
- **Public Spending** — Query detailed expenses (despesas) by year or specific government bodies to monitor how public funds are allocated.
- **Tenders & Bids** — Access information on public tenders (licitações) to stay informed about government procurement processes.
- **Contracts** — Inspect signed contracts and agreements between the municipality and third parties.
- **Personnel & Payroll** — Retrieve data regarding public servants and payroll (servidores) to ensure administrative transparency.

### How it works

1. Subscribe to this server
2. Enter 'PUBLIC' in the access field (this portal uses public data)
3. Start querying municipal data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly gather data for reports on public spending and municipal administration.
- **Citizens & Activists** — monitor government actions and fiscal responsibility directly through conversation.
- **Legal & Compliance Professionals** — verify public contracts and bidding processes without manual portal navigation.


## Available Tools
- **list_bids**: List public tenders and bids (licitações)
- **list_contracts**: List signed contracts (contratos)
- **list_expenses**: List municipality expenses (despesas)
- **list_personnel**: List public servants and payroll (servidores)
- **list_revenues**: List municipality revenues (receitas)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aracaju** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the revenues for Aracaju in January 2024."

**🤖 AI Agent:**
> I've accessed the transparency data for January 2024. The municipality recorded various revenue streams including taxes and federal transfers. Would you like a breakdown by category?

---

**👤 You:**
> "Show me the latest public bids in the city."

**🤖 AI Agent:**
> I've retrieved the list of active public tenders. There are several ongoing bids for infrastructure and services. Do you want to see the details for a specific tender?

---

**👤 You:**
> "What are the expenses for the health department in 2023?"

**🤖 AI Agent:**
> Querying expenses for the health department in 2023... I found the spending records. Would you like to see the total amount or a list of specific payment orders?


## Installation & Usage

To install and use the **Aracaju** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aracaju](https://vinkius.com/mcp/aracaju)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

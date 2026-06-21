# Cuiabá Transparency MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cuiaba-transparency)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cuiaba-transparency-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cuiaba-transparency-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time municipal transparency data for Cuiabá — query expenses, revenues, public personnel, and contracts directly via AI.

## Description
Connect to the **Cuiabá Transparency Portal** and explore municipal public data through natural conversation. This server provides direct access to the city's financial and administrative records.

### What you can do

- **Municipal Expenditures** — List and analyze expenses, including commitments (empenhos), liquidations, and payments for any fiscal year.
- **Revenue Tracking** — Monitor municipal revenue collection, including local taxes and government transfers.
- **Public Personnel** — Access data on public servants, including positions, departments, and salary information.
- **Contracts & Tenders** — Inspect public bids, active contracts, and municipal tenders to ensure oversight.
- **Budget Planning** — Query budget laws and planning instruments like LOA, LDO, and PPA.

### How it works

1. Subscribe to this server
2. Enter your Transparency API Key
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly extract public spending data and personnel lists for investigative reporting.
- **Citizens & Activists** — monitor how municipal resources are being allocated in real-time.
- **Data Analysts** — fetch structured fiscal data for 2023, 2024, and beyond without manual scraping.


## Available Tools
- **list_budget**: List municipal budget information for Cuiabá
- **list_contracts**: List public tenders and contracts for Cuiabá
- **list_expenses**: List municipal expenditures for Cuiabá
- **list_personnel**: List public servants data for Cuiabá
- **list_revenues**: List municipal revenue collection for Cuiabá


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cuiabá Transparency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the municipal expenses for Cuiabá in January 2023."

**🤖 AI Agent:**
> I've retrieved the expenditure data for January 2023. There are several records including health services and infrastructure maintenance. Would you like to see the top 5 largest payments?

---

**👤 You:**
> "Show me the revenue collection for Cuiabá for the year 2023."

**🤖 AI Agent:**
> The revenue data for 2023 shows significant collections from IPTU and ISS, as well as federal transfers. I can break this down by month if you'd like.

---

**👤 You:**
> "Get the list of public servants and their positions in Cuiabá for the current month."

**🤖 AI Agent:**
> I'm accessing the personnel records... I've found the list of active servants, including their departments and roles. Would you like to filter by a specific department like Education or Health?


## Installation & Usage

To install and use the **Cuiabá Transparency** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cuiaba-transparency](https://vinkius.com/mcp/cuiaba-transparency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

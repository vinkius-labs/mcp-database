# Arcadia Plug MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcadia-plug)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arcadia-plug-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arcadia-plug-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access and manage utility data with Arcadia Plug — track accounts, statements, and meters via AI.

## Description
The **Arcadia Plug MCP Server** provides a direct natural language interface to your Arcadia utility data platform. Empower your AI agent to retrieve historical utility bills, monitor meter readings, and audit utility credentials across multiple providers without leaving your workflow.

### Key Features

- **Account Management** — List all linked utility accounts and access detailed metadata including account numbers and statuses.
- **Statement Retrieval** — Access historical utility bills and statements, providing total charges and billing periods.
- **Meter Monitoring** — List individual meters and service points associated with your accounts for granular usage tracking.
- **Credential Oversight** — Track and manage the utility portal credentials used to fetch your data.
- **Unified Data Access** — Interface with hundreds of utility providers through a single, consistent API.
- **Secure OAuth 2.0** — Uses secure Client Credentials flow to ensure safe access to your organization's data.

### Who is this for?

- **Energy Managers** — Quickly audit utility spend and usage across multiple sites and providers.
- **Sustainability Teams** — Gather historical data for ESG reporting and carbon footprint analysis using simple natural language.
- **Financial Analysts** — Monitor utility costs and billing cycles to optimize operational expenses.


## Available Tools
- **get_account_check**: Verify Arcadia account connection
- **get_statement**: Get details for a specific statement
- **list_accounts**: List all utility accounts associated with your organization
- **list_credentials**: List all utility login credentials
- **list_meters**: List all utility meters
- **list_statements**: List historical utility bills/statements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arcadia Plug** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all utility accounts linked to my organization."

**🤖 AI Agent:**
> I've retrieved your accounts. You have 12 linked utility accounts, including 'ConEd - 1234' and 'PG&E - 5678'.

---

**👤 You:**
> "Show me the last 3 statements for the 'ConEd' account."

**🤖 AI Agent:**
> Here are the last 3 statements for your ConEd account. The most recent was for $145.20 for the period ending Jan 31, 2024.

---

**👤 You:**
> "What meters are associated with account ID 'acc_998877'?"

**🤖 AI Agent:**
> Account 'acc_998877' has two meters: an electricity meter (ID: met_1122) and a natural gas meter (ID: met_3344).


## Installation & Usage

To install and use the **Arcadia Plug** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcadia-plug](https://vinkius.com/mcp/arcadia-plug)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

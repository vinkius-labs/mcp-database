# DealHub CPQ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dealhub-cpq)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dealhub-cpq-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dealhub-cpq-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage CPQ and sales via DealHub — create quotes, track opportunity stages, manage users, and sync CRM data directly from any AI agent.

## Description
Connect your **DealHub** account to any AI agent and take full control of your CPQ (Configure, Price, Quote) and sales workflows through natural conversation.

### What you can do

- **Quote Orchestration** — Identify bounded CRM records and generate fresh CPQ sequences linked natively to your Salesforce or HubSpot blocks
- **Live Playbook Access** — Perform structural extraction of quote properties and retrieve secure tokenized URLs to drop users deeply into the Playbook editing flow
- **Opportunity Tracking** — List assigned ongoing deals and read specific synced custom fields mirroring your core CRM limits
- **Deal Management** — Provision highly-available deal shells and updateStage properties instantly across CPQ arrays
- **Quote Status Auditing** — Retrieve explicit cloud logs to parse if PDFs were viewed, signed, or rejected by customers in real-time
- **CRM Synchronization** — Force real-time data ingestion loops against SFDC or MS Dynamics providers to ensure absolute data consistency

### How it works

1. Subscribe to this server
2. Enter your DealHub API Token (found in Admin Mode > API Settings)
3. Start managing your sales quotes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Operations** — monitor quote statuses and manage opportunity stages without manual CRM updates
- **Sales Reps** — create quotes and trigger CRM syncs directly from the IDE or chat during customer negotiations
- **Finance Teams** — audit quote details and verify contract signatures using natural language
- **Revenue Managers** — monitor active sales pipelines and verify rep assignments across the organization


## Available Tools
- **create_opportunity**: Provision a highly-available JSON Payload generating hard Customer bindings
- **create_quote**: 1/quote/create` generating a fresh CPQ sequence linked to a native CRM block.

Identify bounded CRM records inside the Headless DealHub Platform
- **get_opportunity**: Dispatch an automated validation check routing explicit Gateway history
- **get_quote_status**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **list_opportunities**: Enumerate explicitly attached structured rules exporting active Billing
- **list_quotes**: Identify precise active arrays spanning native Gateway auth
- **list_users**: Identify precise active arrays spanning native Hold parsing
- **open_quote**: Perform structural extraction of properties driving active Account logic
- **sync_crm**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **update_opportunity**: Inspect deep internal arrays mitigating specific Plan Math


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DealHub CPQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new quote for opportunity 'opp_abc123' and customer 'Acme Corp'"

**🤖 AI Agent:**
> Quote sequence created! I've linked the new CPQ block to opportunity 'opp_abc123'. You can now use the Playbook URL to define the specific line items and pricing.

---

**👤 You:**
> "What is the status of quote 'dh_quote_789'?"

**🤖 AI Agent:**
> Checking status for 'dh_quote_789'... The PDF has been 'Signed' by the customer. The opportunity stage has been automatically updated to 'Closed Won'.

---

**👤 You:**
> "Sync opportunity 'opp_123' with Salesforce"

**🤖 AI Agent:**
> CRM synchronization triggered! I've forced a data ingestion loop for 'opp_123' against your Salesforce instance. All custom fields and CPQ boundaries are now up to date.


## Installation & Usage

To install and use the **DealHub CPQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dealhub-cpq](https://vinkius.com/mcp/dealhub-cpq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

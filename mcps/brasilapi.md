# BrasilAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brasilapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brasilapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brasilapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access Brazilian institutional data — audit CEP, CNPJ, and banks via AI.

## Description
Empower your AI agent to orchestrate your entire Brazilian institutional research workflow with **BrasilAPI**, the modern interface for Brazilian public data. By connecting BrasilAPI to your agent, you transform complex national lookups into a natural conversation. Your agent can instantly geolocate addresses via CEP, audit company profiles using CNPJ, and retrieve banking information without you ever touching a government portal. Whether you are conducting KYC checks or managing national logistics, your agent acts as a real-time institutional analyst, ensuring your Brazilian data is always verified and up-to-date.

### What you can do

- **CEP Auditing** — Retrieve high-resolution address details for any Brazilian zip code (CEP) and identify neighborhoods and cities instantly.
- **Corporate Oversight** — Audit Brazilian companies using CNPJ to retrieve detailed registration metadata, including tax status and economic activity.
- **Banking Intelligence** — List all banks operating in Brazil and retrieve official codes and clearing metadata.
- **Asset Monitoring** — Query vehicle prices from the FIPE table to understand current market valuations in Brazil.
- **National Monitoring** — List national holidays and retrieve state (UF) metadata from IBGE to coordinate regional operations.

### How it works

1. Subscribe to this server
2. No API Key required (BrasilAPI is a free and open service)
3. Start managing your Brazilian intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Operations** — monitor lead addresses and retrieve verified corporate metadata straight from your workflow.
- **Logistics Managers** — verify delivery regions and audit national holiday constraints without manual searching.
- **Financial Analysts** — perform rapid audits of banking codes and vehicle valuations through natural language.
- **Operations Leads** — automate national data querying to orchestrate cross-functional teams in Brazil smoothly.


## Available Tools
- **list_brazilian_banks**: List all banks operating in Brazil
- **get_cep_details**: Get address details for a Brazilian CEP
- **get_cnpj_details**: Get company details for a Brazilian CNPJ
- **get_fipe_vehicle_price**: Get vehicle price from FIPE table
- **get_brazilian_holidays**: List national holidays in Brazil for a specific year
- **list_brazilian_states**: List all states (UFs) in Brazil via IBGE


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrasilAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get address details for CEP 01001000 using BrasilAPI."

**🤖 AI Agent:**
> I've retrieved the address! It corresponds to Praça da Sé in São Paulo, SP. I can provide the neighborhood and geographic coordinates if you'd like.

---

**👤 You:**
> "Show company details for CNPJ 19131243000197."

**🤖 AI Agent:**
> I've identified that CNPJ as 'VINKIUS'. They are located in São Paulo and their main activity is related to software development. Would you like to see their tax status or partner details?

---

**👤 You:**
> "List all banks in Brazil."

**🤖 AI Agent:**
> I've scanned the bank catalog. There are over 300 institutions listed, including Banco do Brasil, Itaú, and Bradesco. I can provide the official codes for any of them.


## Installation & Usage

To install and use the **BrasilAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brasilapi](https://vinkius.com/mcp/brasilapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

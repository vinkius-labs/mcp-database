# ANP (Revendedores de Combustíveis) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anp-revendedores-de-combustiveis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anp-revendedores-de-combustiveis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian fuel and LPG reseller data from ANP — query gas stations and cooking gas providers by location or CNPJ.

## Description
Connect to the **ANP (Agência Nacional do Petróleo, Gás Natural e Biocombustíveis)** database to retrieve real-time information about authorized resellers across Brazil through natural conversation.

### What you can do

- **Automotive Fuel Resellers** — Search for gas stations using filters like state (UF), municipality, or specific CNPJ via the `list_combustivel_resellers` tool.
- **LPG (Cooking Gas) Resellers** — Locate authorized GLP distributors and resellers nationwide using the `list_glp_resellers` tool.
- **Public Data Verification** — Verify the registration and status of fuel providers directly from the official regulatory source.
- **Geographic Analysis** — List all resellers within a specific city or state to understand regional coverage and availability.

### How it works

1. Subscribe to this server
2. Enter your ANP API Access Key (if required)
3. Start querying Brazilian energy and fuel data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Analysts** — track the distribution of fuel resellers in different regions for competitive analysis
- **Logistics & Fleet Managers** — identify authorized refueling points and verify reseller credentials
- **Compliance Officers** — verify the legal status of resellers against official government records


## Available Tools
- **list_combustivel_resellers**: Can be filtered by CNPJ, state (UF), and municipality.

List automotive fuel resellers
- **list_glp_resellers**: Can be filtered by CNPJ, state (UF), and municipality.

List LPG (cooking gas) resellers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ANP (Revendedores de Combustíveis)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all automotive fuel resellers in the city of 'São Paulo', SP."

**🤖 AI Agent:**
> I've retrieved the list of authorized fuel resellers in São Paulo (SP). There are multiple entries; would you like to see the first page of results or filter by a specific CNPJ?

---

**👤 You:**
> "Find LPG (cooking gas) resellers in the state of Rio de Janeiro (RJ)."

**🤖 AI Agent:**
> Searching for GLP resellers in RJ... I found several authorized distributors. You can further narrow this down by municipality if needed.

---

**👤 You:**
> "Check the status of the reseller with CNPJ 00000000000191."

**🤖 AI Agent:**
> Querying ANP for CNPJ 00000000000191... I have found the registration details. The reseller is currently listed as authorized for automotive fuel sales.


## Installation & Usage

To install and use the **ANP (Revendedores de Combustíveis)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anp-revendedores-de-combustiveis](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

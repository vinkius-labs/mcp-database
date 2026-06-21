# ANP (Revendedores de Combustíveis) MCP Server

Access official Brazilian fuel and LPG reseller data from ANP — query gas stations and cooking gas providers by location or CNPJ.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)

## Overview
**Category:** data-analytics
**Tools Count:** 2

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


## Installation & Usage

To install and use the **ANP (Revendedores de Combustíveis)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anp-revendedores-de-combustiveis](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

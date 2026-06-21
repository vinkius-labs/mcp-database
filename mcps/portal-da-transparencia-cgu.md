# Portal da Transparência (CGU) MCP Server

Access Brazilian government transparency data — query social benefits (Bolsa Família, Auxílio Emergencial), public expenses, and SIAFI organizations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/portal-da-transparencia-cgu)

## Overview
**Category:** data-analytics
**Tools Count:** 9

## Description
Connect to the **Portal da Transparência (CGU)** and audit Brazilian public spending and social programs directly through your AI agent.

### What you can do

- **Social Benefits** — Query availability and withdrawals for Bolsa Família and Auxílio Emergencial using CPF, NIS, or municipality codes.
- **Public Expenses** — Fetch detailed expense documents and payment records for specific beneficiaries or companies.
- **Institutional Data** — List and search for government organizations registered in the SIAFI system.
- **Environmental & Labor Grants** — Access records for Seguro Defeso using specific identification codes.
- **Local Auditing** — Analyze benefit distribution across different Brazilian municipalities for regional insights.

### How it works

1. Subscribe to this server
2. Enter your CGU API Key (obtained from the official portal)
3. Start auditing public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly verify government transfers and social program distributions without manual portal navigation.
- **Public Auditors** — cross-reference expense documents and beneficiary data directly within your analysis workflow.
- **Civic Tech Developers** — build tools that monitor public spending using real-time government data.


## Available Tools
- **get_auxilio_emergencial_beneficiario_por_municipio**: Restricted API limit applies.

Get Auxilio Emergencial beneficiaries by municipality
- **get_auxilio_emergencial_por_cpf_ou_nis**: Restricted API limit applies.

Get Auxilio Emergencial by CPF or NIS
- **get_auxilio_emergencial_por_municipio**: Restricted API limit applies.

Get Auxilio Emergencial by municipality
- **get_bolsa_familia_disponivel_por_cpf_ou_nis**: Restricted API limit applies.

Get available Bolsa Familia by CPF or NIS
- **get_bolsa_familia_por_municipio**: Restricted API limit applies.

Get Bolsa Familia by municipality
- **get_bolsa_familia_sacado_por_nis**: Restricted API limit applies.

Get withdrawn Bolsa Familia by NIS
- **get_despesas_documentos_por_favorecido**: Restricted API limit applies.

Get expense documents by beneficiary
- **get_orgaos_siafi**: Supports pagination.

List SIAFI organizations
- **get_seguro_defeso_codigo**: Restricted API limit applies.

Get Seguro Defeso by code


## Installation & Usage

To install and use the **Portal da Transparência (CGU)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portal-da-transparencia-cgu](https://vinkius.com/mcp/portal-da-transparencia-cgu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

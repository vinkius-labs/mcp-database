# Portal da Transparência (CGU) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portal-da-transparencia-cgu)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/portal-da-transparencia-cgu-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/portal-da-transparencia-cgu-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazilian government transparency data — query social benefits (Bolsa Família, Auxílio Emergencial), public expenses, and SIAFI organizations.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portal da Transparência (CGU)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check Bolsa Família availability for CPF 000.000.000-00."

**🤖 AI Agent:**
> I've checked the records for that CPF. There is an available benefit for the current month in the amount of R$ 600.00. Would you like to see the payment history?

---

**👤 You:**
> "List all SIAFI organizations on page 1."

**🤖 AI Agent:**
> Fetching the first page of SIAFI organizations... I found entries including the Ministry of Education (MEC), Ministry of Health, and the Presidency of the Republic. Do you need details on a specific one?

---

**👤 You:**
> "Show expense documents for beneficiary 'Empresa Exemplo LTDA'."

**🤖 AI Agent:**
> I found 3 expense documents for 'Empresa Exemplo LTDA'. The most recent is a payment of R$ 50,000.00 for technical services. Would you like the document IDs?


## Installation & Usage

To install and use the **Portal da Transparência (CGU)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portal-da-transparencia-cgu](https://vinkius.com/mcp/portal-da-transparencia-cgu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

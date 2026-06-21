# Paraíba Open Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paraiba-open-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/paraiba-open-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/paraiba-open-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official public spending, budget, and payroll data from the State of Paraíba, Brazil, directly through your AI agent.

## Description
The **Paraíba MCP Server** connects your AI agent to the official Dados Abertos portal of the State of Paraíba. This integration allows for real-time auditing and analysis of public finances, government contracts, and personnel spending through natural conversation.

### What you can do

- **Budget & Finance** — Query budget allocations (`get_dotacao`), liquidations (`get_liquidacao`), and revenue execution or forecasts.
- **Public Spending** — Inspect commitment notes (`get_empenho`), daily allowances for public servants (`get_diarias`), and payment authorizations.
- **Human Resources** — Access detailed payroll summaries (`get_folha_pagamento`) to monitor state personnel costs.
- **Contracts & Agreements** — List and analyze government contracts (`get_contratos`) and outstanding payables (Restos a Pagar).
- **Institutional Structure** — Retrieve information about management units, government actions, and resource sources.

### How it works

1. Subscribe to this server
2. Enter your API access token for the Paraíba data proxy
3. Start auditing public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — Instantly aggregate spending data for investigative reports without manual CSV exports.
- **Public Auditors & Lawyers** — Cross-reference contracts and payment authorizations directly from your workspace.
- **Engaged Citizens** — Exercise transparency by asking simple questions about how state resources are allocated.


## Available Tools
- **get_acao_governamental**: Get Ação Governamental (Government Action) data
- **get_autorizacao_pagamento**: Get Autorizações de Pagamento (Payment Authorizations) data
- **get_contratos_aditivos**: Get Aditivos de Contratos (Contract Addendums) data
- **get_contratos**: Get Contratos (Contracts) data
- **get_convenios**: Get Convênios (Covenants/Agreements) data
- **get_diarias**: Get Despesa Orçamentária - Diárias (Daily Allowances) data
- **get_dotacao**: Get Dotação Orçamentária (Budget Allocation) data
- **get_elemento_despesa**: Get Elemento da Despesa (Expense Element) data
- **get_empenho**: Get Despesa Orçamentária - Notas de Empenho (Commitment Notes) data
- **get_folha_pagamento**: Get Resumo da Folha de Pagamento (Payroll Summary) data
- **get_fonte_recurso**: Get Fonte de Recurso (Resource Source) data
- **get_funcao**: Get Função (Function) data
- **get_liquidacao**: Get Liquidação (Liquidation) data
- **get_modalidade_licitacao**: Get Modalidade de Licitação (Bidding Modality) data
- **get_receitas_execucao**: Get Receitas - Execução (Revenue Execution) data
- **get_receitas_previsao**: Get Receitas - Previsão (Revenue Forecast) data
- **get_restos_a_pagar**: Get Restos a Pagar (Outstanding Payables) data
- **get_subfuncao**: Get Sub Função (Sub-function) data
- **get_unidade_gestora**: Get Unidade Gestora (Managing Unit) data
- **get_unidade_orcamentaria**: Get Unidade Orçamentária (Budgetary Unit) data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paraíba Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the budget allocation (dotação) for Paraíba in 2024."

**🤖 AI Agent:**
> I've retrieved the budget allocation data for 2024. The total authorized amount is distributed across various departments. Would you like a breakdown by month or by management unit?

---

**👤 You:**
> "What was the payroll summary for March 2024?"

**🤖 AI Agent:**
> For March 2024, the payroll summary shows the total gross and net values for state employees. I can provide the specific totals for active, inactive, and pensioned personnel if needed.

---

**👤 You:**
> "List the daily allowances (diárias) paid in January 2024."

**🤖 AI Agent:**
> I found the records for daily allowances in January 2024. The data includes the names of recipients, the purpose of travel, and the amounts paid. Should I summarize the top spending units?


## Installation & Usage

To install and use the **Paraíba Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paraiba-open-data](https://vinkius.com/mcp/paraiba-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

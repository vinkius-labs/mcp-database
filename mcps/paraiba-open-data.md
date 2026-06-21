# Paraíba Open Data MCP Server

Access official public spending, budget, and payroll data from the State of Paraíba, Brazil, directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/paraiba-open-data)

## Overview
**Category:** data-analytics
**Tools Count:** 20

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


## Installation & Usage

To install and use the **Paraíba Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paraiba-open-data](https://vinkius.com/mcp/paraiba-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

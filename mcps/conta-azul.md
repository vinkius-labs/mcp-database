# Conta Azul MCP Server

Manage Brazilian ERP via Conta Azul — track customers, products, services, sales, and monitor financial contracts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/conta-azul)

## Overview
**Category:** erp-operations
**Tools Count:** 15

## Description
Connect your **Conta Azul** account to any AI agent and take full control of your Brazilian business ERP and financial management through natural conversation.

### What you can do

- **Customer Management** — List and search for customers (PJ/PF), audit fiscal documents (CNPJ/CPF), and create new financial entities natively
- **Inventory & Services** — Map physical products (SKU) and intangible services, retrieve pricing, units of measure, and create new billable components
- **Sales Monitoring** — List continuous logs of confirmed sales, retrieve detailed accounting matrices for units, and verify invoice statuses
- **Recurrence Tracking** — Audit financial contracts and automatic agreements to monitor monthly/annual technical debt and expiration dates
- **Fiscal Compliance (NF-e)** — Retrieve governmental emissions records (NF-e) and validate SEFAZ approval statuses for product invoices
- **Financial Structure** — Access hierarchical category trees (DRE) and map bank accounts to reconcile monetary positions and internal cash flow

### How it works

1. Subscribe to this server
2. Enter your Conta Azul OAuth 2.0 Access Token (found in the Developer Portal under your Application)
3. Start managing your Brazilian ERP from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners (Brazil)** — monitor sales volume and customer balances without logging into the full ERP interface
- **Finance Teams** — audit bank accounts, categories, and financial contracts using natural language
- **Sales Reps** — check customer fiscal details and product availability during negotiations
- **Accounting Operations** — verify NF-e statuses and reconcile billing logs directly from the workspace


## Available Tools
- **list_customers**: Listar base de clientes paginada extraindo entidades corporativas no ERP
- **get_customer**: Extrair perfil estático financeiro via UUID rastreando limites PF/PJ explícitos
- **search_customers**: Pesquisar perfis corporativos/fiscais comparando documentos restritos via CPF/CNPJ
- **create_customer**: Injetar novo registro financeiro PF/PJ definindo estrutura formal dentro do ERP
- **list_products**: Mapear itens físicos catalogados incluindo valores de SKU extraídos estaticamente
- **get_product**: Ler dados de um item físico individual incluindo limite e unidade de medida
- **create_product**: Mapear bens tangíveis definindo novos componentes faturáveis em Real financeiro
- **list_services**: Ler prestação categorizada cobrável na estrutura contábil faturada paginada
- **create_service**: Inserir prestação ativa intangível estritamente precificada na contabilidade
- **list_sales**: Listar logs contínuos extraídos avaliando faturas pendentes emitidas no fluxo
- **get_sale**: Visualizar blocos confirmados incluindo matrizes exatas contábeis da venda UUID
- **list_contracts**: Pesquisar recorrências atestando acordos automáticos limitando vencimentos
- **list_nfe**: Buscar listagem governamental acoplada de emissões NF (Notas de Produto)
- **list_categories**: g. Despesas, Receitas) que formam a espinha dorsal de DRE validada base ContaAzul.

Determinar limites contábeis de Plano Analítico nativo classificando recursos
- **list_bank_accounts**: Mapear bancos físicos conciliando integração extraindo posições monetárias


## Installation & Usage

To install and use the **Conta Azul** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conta-azul](https://vinkius.com/mcp/conta-azul)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

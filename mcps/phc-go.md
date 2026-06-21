# PHC GO MCP Server

Equip your AI agent to control your PHC GO ERP. Query customers, retrieve real-time stocks, map taxes, and issue documents conversationally.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/phc-go)

## Overview
**Category:** erp-operations
**Tools Count:** 16

## Description
Connect your **PHC GO** enterprise ecosystem to your AI agent and manage operations, invoicing, and logistics through natural language commands natively.

### What you can do

- **Entity Management** — Retrieve master data such as `list_customers` and natively `create_customer` directly from your chat context.
- **Inventory & Logistics** — Pull active article sheets with `list_products`, or audit material counts instantly using `list_stocks` and `list_warehouses`.
- **Billing & Finance** — Dynamically execute the `create_document` endpoint to issue invoices/estimates, and reconcile using `list_current_accounts` and `list_taxes`.
- **Sales Ecosystem** — Quickly fetch configuration records like `list_series` and `list_payment_methods` to standardize business logic via intelligent agents.

### How it works

1. Subscribe to this server
2. Enter your PHC GO Backend URL and your generated API Access Token
3. Start fetching stock items and drafting financial documents directly from Claude, Cursor, or your chosen AI interface

### Who is this for?

- **Finance Directors** — check outstanding current accounts directly from the IDE and orchestrate document extraction without logging into the ERP.
- **Sales Representatives** — securely consult real-time stock availability out on the road before confirming a sale with the customer.
- **Developers & SysOps** — programmatically query the PHC API layer to inspect product metrics, schemas, and endpoints during rapid feature development.


## Available Tools
- **list_customers**: Listar todas as entidades/clientes registados no PHC GO
- **get_customer_details**: Obter detalhes completos de um cliente/entidade pelo ID
- **search_customers**: Pesquisar clientes por nome, NIF ou código
- **create_customer**: Criar um novo cliente/entidade no PHC GO
- **list_products**: Listar todos os artigos e serviços registados no PHC GO
- **get_product_details**: Obter detalhes de um artigo/serviço pelo ID
- **create_product**: Criar um novo artigo ou serviço no PHC GO
- **list_documents**: Listar documentos comerciais do PHC GO por tipo (FT=Fatura, NC=Nota Crédito, RC=Recibo, ORC=Orçamento, ECL=Encomenda, GR=Guia Remessa)
- **get_document_details**: Obter detalhes completos de um documento comercial (fatura, nota crédito, recibo, etc) incluindo linhas
- **create_document**: Criar um novo documento comercial no PHC GO (fatura, orçamento, encomenda, etc)
- **list_stocks**: Consultar movimentos de stock. Opcionalmente filtrar por artigo
- **list_current_accounts**: Consultar a conta corrente de clientes (saldos e movimentos pendentes)
- **list_taxes**: Listar taxas de IVA e impostos configurados no PHC GO
- **list_series**: Listar séries de numeração de documentos (FT 2026/, NC 2026/, etc)
- **list_payment_methods**: Listar métodos de pagamento configurados (Transferência, MB, MBWay, Cheque)
- **list_warehouses**: Listar armazéns configurados para gestão de stock


## Installation & Usage

To install and use the **PHC GO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phc-go](https://vinkius.com/mcp/phc-go)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

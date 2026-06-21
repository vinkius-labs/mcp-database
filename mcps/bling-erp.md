# Bling ERP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bling-erp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bling-erp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bling-erp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Connect Bling ERP via AI — manage inventory, process orders, issue Brazilian tax documents (NF-e), and track accounts directly from your agent.

## Description
Connect your **Bling ERP** API token to any AI agent and integrate Brazil's leading cloud-based business management system directly into your conversational workflow.

### What you can do

- **Contact & Product Operations** — Create and list deeply nested catalogs of Contacts (Suppliers/Clients) and Products, tracing correct SKUs, categories, and warehouses.
- **Order Processing** — List Sales Orders bridging eCommerce streams directly to inventory, and explore incoming Purchase Orders to suppliers.
- **Tax Documents (Brasil)** — Monitor SEFAZ legal endpoints querying arrays for issued Product Invoices (NF-e), Consumer Invoices (NFC-e), and Service Invoices (NFS-e).
- **Financial Ledgering** — Pull aggregated general ledgers analyzing Accounts Payable, Accounts Receivable (Boletos/PIX), and strictly mapped financial groupings.

### How it works

1. Subscribe to this server
2. Enter your Bling Access Token
3. Start running ERP operational logic from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **E-Commerce Operators** — list incoming sales orders and sync product stock intelligently using text commands.
- **Financial Managers** — consult outstanding accounts receivable and evaluate incoming bills instantly.
- **Logistics Teams** — search warehouse logic and map client logistics strictly prior to issuing an NF-e.


## Available Tools
- **listar_contatos**: Listar todos os contatos (clientes, fornecedores, transportadoras) cadastrados no Bling
- **consultar_contato**: Consultar dados completos de um contato pelo ID
- **incluir_contato**: Cadastrar novo contato (cliente/fornecedor) no Bling
- **listar_produtos**: Listar todos os produtos e serviços cadastrados no Bling
- **consultar_produto**: Consultar detalhes de um produto pelo ID
- **incluir_produto**: Cadastrar novo produto no Bling
- **categorias_produtos**: Listar as categorias de produtos cadastradas
- **listar_pedidos_venda**: Listar todos os pedidos de venda do Bling
- **consultar_pedido**: Consultar detalhes completos de um pedido de venda (itens, valores, situação)
- **listar_pedidos_compra**: Listar todos os pedidos de compra
- **listar_nfe**: Listar NF-e (Notas Fiscais Eletrônicas de Produto) emitidas
- **consultar_nfe**: Consultar detalhes de uma NF-e (itens, valores, situação)
- **listar_nfce**: Listar NFC-e (Notas Fiscais de Consumidor Eletrônicas — cupom fiscal)
- **listar_nfse**: Listar NFS-e (Notas Fiscais de Serviço Eletrônicas)
- **contas_receber**: Listar contas a receber (cobranças, boletos, PIX)
- **contas_pagar**: Listar contas a pagar (fornecedores, despesas operacionais)
- **categorias_financeiras**: Listar categorias de receitas e despesas (plano de contas)
- **listar_depositos**: Listar depósitos/armazéns configurados para gestão de estoque


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bling ERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 registered products in my Bling account."

**🤖 AI Agent:**
> I queried your product catalog via API v3. Here are the items: 1. 'Nike Running Shoes' (SKU: 991, $120.00), 2. 'Wireless Mouse' (SKU: 992, $35.00)...

---

**👤 You:**
> "Check the active Accounts Payable for this month. What vendor bills are pending?"

**🤖 AI Agent:**
> I checked the ledger using the accounts payable component. There is an outstanding invoice matching Vendor ID `5541` equivalent to $400.00 due this forthcoming Friday.

---

**👤 You:**
> "Has the NF-e for the sales order ID `445566` been fully issued yet under SEFAZ?"

**🤖 AI Agent:**
> I parsed the order array. Yes, the invoice is marked internally as 'Issued'. The exact Brazilian legal protocol access key connected to the event states 3522-...


## Installation & Usage

To install and use the **Bling ERP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bling-erp](https://vinkius.com/mcp/bling-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

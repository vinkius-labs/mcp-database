# Bling ERP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bling-erp)
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


## ❓ FAQ

**Q: Does the integration support checking Brazilian Tax Invoices (NFe)?**
Yes. Your AI agent natively interacts with API v3 executing tools like 'listar_nfe', 'listar_nfce', and 'listar_nfse', actively checking their valid SEFAZ digital status and exact final values.

**Q: Can I actually create new Products or Contacts via my AI agent chat?**
Yes. Utilizing the 'incluir_produto' and 'incluir_contato' tools, your AI can ingest unstructured raw data from an email or document and flawlessly mint it into structural tables on your Bling backend database.

**Q: Can I check my Accounts Receivable and open Boletos directly?**
Absolutely. The agent holds explicit operational authority across the 'contas_receber' tool, strictly reporting open invoices, boletos, PIX items, and the total value currently pending payment globally.

**Q: Can I check stock levels across multiple warehouses?**
Yes! Your agent can use the 'list_depositos' tool to see where your inventory is physically located across your different warehouses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bling-erp](https://vinkius.com/mcp/bling-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bling ERP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bling-erp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bling ERP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bling-erp": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

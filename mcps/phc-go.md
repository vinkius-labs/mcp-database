# PHC GO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phc-go)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to control your PHC GO ERP. Query customers, retrieve real-time stocks, map taxes, and issue documents conversationally.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PHC GO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the available stock for 'Macbook Pro M3' across all warehouses."

**🤖 AI Agent:**
> I checked the ERP. We currently hold 42 units of 'Macbook Pro M3': 30 units at Warehouse North and 12 units at Central Logistics.

---

**👤 You:**
> "Create a new customer profile for 'Acme Corp' and fetch their assigned customer ID."

**🤖 AI Agent:**
> Understood. The entity 'Acme Corp' was successfully pushed to PHC GO configuration. Their internal Customer ID assigns to `CUST-989201`.

---

**👤 You:**
> "Examine our outstanding current accounts from January to spot pending vendor debts."

**🤖 AI Agent:**
> According to the ERP 'list_current_accounts' query, there are 4 open vendor invoices flagged as overdue from January. Here's a table summarizing the debtors and owed amounts.


## ❓ FAQ

**Q: Can my AI actively search for a specific customer before creating an invoice?**
Yes. It can sequentially execute `search_customers` to find the precise Unique ID of the customer using fuzzy name matching, and subsequently inject that accurate payload into `create_document` without human error.

**Q: Is 'list_stocks' showing data in real-time?**
Yes. Since this operates as a direct pass-through via the MCP to the PHC GO platform API, all stock matrices, warehouse item counts, and current accounts represent the exact live state of your corporate database in the split second the AI requests it.

**Q: Can I query products that exist across multiple warehouses?**
Absolutely. By commanding the agent to align returns from both `list_products` and `list_warehouses` against `list_stocks`, your LLM can map out a matrix comparing which warehouse holds the higher volume of the targeted SKUs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phc-go](https://vinkius.com/mcp/phc-go)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PHC GO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `phc-go` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PHC GO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phc-go": {
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

# Omie ERP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omie-erp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Omie ERP data via API — list clients, products, sales orders, financial accounts, and inventory directly from any AI agent.

## Description
Connect your **Omie ERP** account to any AI agent and take full control of your business management workflows through natural conversation.

### What you can do

- **Client Management** — List, create, update, and inspect clients (customers, suppliers) with full contact and tax information
- **Product Catalog** — Browse products and services, check details, create new items, and monitor stock levels
- **Sales Orders** — List, create, and inspect sales orders with line items, pricing, and payment terms
- **Financial Monitoring** — Track accounts receivable and payable to monitor cash flow and identify overdue items
- **Bank Accounts** — List configured bank accounts and check balances for financial reconciliations
- **Inventory Control** — Monitor stock levels, check product availability, and identify items needing reorder
- **Services Catalog** — List and manage non-physical services offered to clients

### How it works

1. Subscribe to this server
2. Enter your Omie App Key and App Secret from the developer portal
3. Start managing clients, products, orders, and finances from Claude, Cursor, or any MCP-compatible client

No more navigating the Omie dashboard for every data lookup. Your AI acts as a dedicated ERP assistant.

### Who is this for?

- **Business Owners** — instantly check client details, product availability, and financial status without opening the ERP
- **Sales Teams** — create and inspect sales orders directly from conversations, verify pricing and stock levels
- **Financial Managers** — monitor accounts receivable/payable and identify overdue invoices or bills
- **Operations Staff** — check inventory levels, create clients, and manage product catalog efficiently


## Available Tools (16)
- **create_client**: You must provide at minimum the business name (razao_social)
and CNPJ/CPF. Optional fields include trade name, address, contacts, email, phone, payment terms, and credit limits.
The response includes the newly created client code which can be used for future references.
Data must be provided as a JSON object matching Omie's client schema.

Create a new client (customer/supplier) in Omie ERP
- **create_product**: You must provide at minimum the product code (codigo_produto)
and description. Optional fields include NCM, unit, cost price, sale price, stock quantity, and tax configuration.
The response includes the newly created product details. Data must be provided as a JSON object matching Omie's product schema.

Create a new product in Omie ERP
- **create_sales_order**: You must provide the client code (codigo_cliente) and at least
one line item with product code, quantity, and price. Optional fields include discounts, taxes, shipping info,
and payment terms. The response includes the newly created order code. Data must be provided as JSON matching Omie's order schema.

Create a new sales order (pedido de venda) in Omie ERP
- **get_client**: Use the client_id (codigo_cliente) obtained from list_clients to inspect full client details.
This is useful for verifying client data before creating orders or invoices.

Get detailed information about a specific client
- **get_product**: Use the product_code (codigo_produto) obtained from
list_products to inspect full product details. This is useful for verifying product data before creating orders.

Get detailed information about a specific product
- **get_sales_order**: Use the order_id (codigo_pedido) obtained from
list_sales_orders to inspect full order details. This is useful for verifying order data before invoicing.

Get detailed information about a specific sales order
- **get_stock_summary**: Use the product_code (codigo_produto) obtained from list_products to inspect stock details.
This helps determine if a product is available for sale or needs reordering.

Get stock summary for a specific product
- **list_accounts_payable**: Each entry includes supplier, due date, amount, status (open, paid, overdue), and payment method.
You can optionally specify page number and records per page. Use this to monitor outgoing payments
and identify bills that are due or overdue.

List all accounts payable (contas a pagar) in Omie ERP
- **list_accounts_receivable**: Each entry includes client, due date, amount, status (open, paid, overdue), and payment method.
You can optionally specify page number and records per page. Use this to monitor incoming payments
and identify overdue invoices that need follow-up.

List all accounts receivable (contas a receber) in Omie ERP
- **list_bank_accounts**: Each account includes bank name, agency, account number, and current balance.
Use this to verify which bank accounts are available for financial transactions and reconciliations.

List all bank accounts (contas correntes) configured in Omie ERP
- **list_clients**: Each client includes business name (razao_social), trade name (nome_fantasia), CNPJ/CPF, contact information,
address, and client code. You can optionally specify page number and records per page (default: 50).
Use this to browse your client database or find a specific client by name or document.

List all clients (customers, suppliers) in Omie ERP
- **list_products**: You can optionally specify page number and records per page (default: 50).
Use this to browse your product catalog or find a specific product by code or description.

List all products and services in Omie ERP
- **list_sales_orders**: You can optionally specify page number and records per page.
Use this to browse your sales pipeline or find a specific order by number or client.

List all sales orders (pedidos de venda) in Omie ERP
- **list_services**: Services are non-physical offerings sold to clients (consulting, maintenance, etc.).
You can optionally specify page number and records per page. Use this to browse your service catalog.

List all services (serviços) registered in Omie ERP
- **list_stock**: Each entry includes product code, description, quantity in stock, minimum stock level, and warehouse location.
You can optionally specify page number and records per page. Use this to monitor inventory levels
and identify products that need reordering.

List stock/inventory levels for all products in Omie ERP
- **update_client**: You must provide the client_id (codigo_cliente)
and the fields to update. Only the fields provided in client_data will be updated.
This is useful for correcting client information, updating addresses, or changing payment terms.
The client_id must exist in the system.

Update an existing client in Omie ERP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omie ERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my clients and show me their total outstanding balances."

**🤖 AI Agent:**
> I've retrieved your client list. You have 247 clients registered. Top clients by outstanding balance:
1. **TechCorp Ltda** (CNPJ: 12.345.678/0001-90) — R$ 45,230.00 outstanding
2. **Distribuidora ABC** (CNPJ: 98.765.432/0001-10) — R$ 28,900.00 outstanding
3. **Consultoria XYZ** (CPF: 123.456.789-00) — R$ 12,450.00 outstanding

Would you like the full details of any specific client or their payment history?

---

**👤 You:**
> "Create a new sales order for client TechCorp with 5 units of product 'Consulting Hours' at R$ 150/hour."

**🤖 AI Agent:**
> I've created the sales order successfully:
- **Order Code**: PV-20260407-001
- **Client**: TechCorp Ltda (CNPJ: 12.345.678/0001-90)
- **Item**: Consulting Hours — 5 units × R$ 150.00 = R$ 750.00
- **Total**: R$ 750.00
- **Status**: Open

The order is now in Omie and ready for invoicing. Would you like to generate the invoice (NF-e) for this order?

---

**👤 You:**
> "Show me all overdue accounts payable and the total amount owed."

**🤖 AI Agent:**
> I found 5 overdue accounts payable totaling R$ 18,750.00:

1. **Supplier ABC** — R$ 5,200.00 — Due: 2026-03-15 (23 days overdue)
2. **Office Rent** — R$ 4,500.00 — Due: 2026-03-20 (18 days overdue)
3. **Internet Provider** — R$ 350.00 — Due: 2026-03-25 (13 days overdue)
4. **Software License** — R$ 2,700.00 — Due: 2026-04-01 (6 days overdue)
5. **Cleaning Services** — R$ 6,000.00 — Due: 2026-04-05 (2 days overdue)

Would you like me to help you prioritize which payments to process first?


## ❓ FAQ

**Q: How do I get Omie API credentials (App Key and App Secret)?**
Log in to your Omie ERP account, go to **Configurações > Aplicativos** (Settings > Applications), and create a new application. Omie will automatically generate an **App Key** and **App Secret** for you. Copy both values immediately — the App Secret is shown only once. Paste them into the respective fields below. These credentials are used to authenticate all API requests.

**Q: Can I create new clients and products through this integration?**
Yes! Use the `create_client` tool to add new clients (customers/suppliers) and `create_product` to add new products to your Omie catalog. You'll need to provide the data as JSON objects matching Omie's schema. The AI agent can help you structure the data correctly. After creation, you'll receive the new client or product code for future reference.

**Q: How can I monitor overdue invoices and payments?**
Use `list_accounts_receivable` to see all money owed to your company, and `list_accounts_payable` to see all money you owe. Each entry includes the due date, amount, and status. You can filter and identify overdue items by comparing the due date with today's date. The AI agent can help you analyze the results and highlight which invoices need immediate attention.

**Q: What ERP modules are accessible through this API?**
This integration covers the core Omie modules: **Clients** (customers, suppliers, transporters), **Products & Services** (catalog management), **Sales Orders** (pedidos de venda), **Accounts Receivable** (contas a receber), **Accounts Payable** (contas a pagar), **Bank Accounts** (contas correntes), and **Inventory/Stock** (estoque). Additional modules like NF-e, NFS-e, CRM, and purchases are available through Omie's full API but may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omie-erp](https://vinkius.com/mcp/omie-erp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Omie ERP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `omie-erp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Omie ERP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omie-erp": {
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

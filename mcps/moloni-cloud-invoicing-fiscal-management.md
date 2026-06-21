# Moloni (Cloud Invoicing & Fiscal Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moloni-cloud-invoicing-fiscal-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage certified invoicing via Moloni — track customers by VAT/NIF, audit invoices, and monitor stock levels.

## Description
Connect your **Moloni** account to any AI agent and take full control of your certified cloud invoicing, commercial management, and fiscal compliance through natural conversation.

### What you can do

- **Customer CRM (VAT/NIF)** — Search for registered customers by name or exact fiscal NIF and retrieve detailed profiles including billing addresses and legal dependencies directly from your agent
- **Invoice & Document Audit** — List and retrieve detailed representations of certified invoices (FT), invoice-receipts (FR), and credit notes (NC) to monitor your sales and tax distributions securely
- **Product & Stock Tracking** — List your complete catalog of articles and services, including base pricing and VAT configurations, and monitor real-time stock movements and warehousing logs natively
- **Commercial Estimations** — Access and audit active quotes and proforma estimates to track pending client approvals and sales pipeline boundaries securely
- **Fiscal Configuration** — Retrieve legal reference IDs for taxes, measurement units, and payment methods required for generating compliant mutations across Portuguese and Spanish jurisdictions
- **Customer Registration** — Instantly create new client records with full fiscal metadata, including zip-coded addresses and country mappings, to prepare your environment for rapid invoicing
- **Metadata Inspection** — Deep-dive into specific Document or Product IDs to retrieve precise JSON payloads and unit mapping constants instantly

### How it works

1. Subscribe to this server
2. Enter your Moloni Access Token and Company ID
3. Start managing your business operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners** — monitor sales flows and audit fiscal documents through natural conversation without manual dashboard navigation
- **Accountants** — retrieve detailed invoice data and tax breakdowns directly from your workspace to streamline financial reporting
- **E-commerce Managers** — verify stock levels and manage customer fiscal profiles efficiently to maintain high-performance digital commerce


## Available Tools
- **list_customers**: Listar todos os clientes registados na empresa Moloni
- **get_customer_by_vat**: Pesquisar exato cliente pelo seu NIF fiscal
- **create_customer**: Registar formalmente novo cliente no Moloni
- **update_customer**: Atualizar registo de dados fiscais num cliente existente
- **list_products**: Listar todos os artigos e stock de serviços Moloni
- **get_product**: Obter pormenores unitários e ID de taxas de um serviço
- **create_product**: Criar registo de novo artigo faturável base
- **list_product_categories**: Listar hierarquia de categorias guardando os produtos
- **list_product_stocks**: Consultar movimentos brutos auditáveis do stock
- **list_invoices**: Listar faturas simples já finalizadas ou abertas AT
- **get_invoice**: Obter detalhe intrínseco (items e IVAs) duma exata Fatura
- **list_invoice_receipts**: Listar FRV (Fatura-Recibo equivalentes portugueses)
- **list_receipts**: Listar RCs (Recibos líquidos de regularização liquidados)
- **list_credit_notes**: Listar NCs legais (Notas de Crédito estornos)
- **list_delivery_notes**: Listar GTs puras (Guias de Transporte físicas)
- **list_estimates**: Listar orçamentos simulados (Proformas/Orçamentos)
- **list_taxes**: Listar impostos e isenções IVA ativos
- **list_payment_methods**: Listar IDs de pagamento associados à AT
- **list_measurement_units**: Listar unidades métricas configuradas formalmente
- **list_countries**: Listar referências ISO IDs e jurisdições fiscais


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moloni (Cloud Invoicing & Fiscal Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the customer with NIF '123456789' in my Moloni account"

**🤖 AI Agent:**
> Retrieving fiscal entity… I've identified the customer 'Innovative Tech Solutions Lda' (ID: 98765) matching NIF 123456789. The account is active and has a billing address in Lisbon. Would you like to see their last 3 invoices?

---

**👤 You:**
> "List all pending estimates (budgets) from this month"

**🤖 AI Agent:**
> I've retrieved 5 active estimates generated this month. Highlights include 'Web Design Quote' (€1,200), 'Monthly Maintenance' (€450), and 'Hardware Provisioning' (€3,500). None have been converted to invoices yet. Would you like to check the details for the design quote?

---

**👤 You:**
> "Check the stock level for product 'Standard SaaS License' (ID: 13579)"

**🤖 AI Agent:**
> Retrieving inventory for ID 13579… You currently have 45 units available in your main warehouse. The last movement was an outbound sale 2 hours ago. There are no pending delivery notes for this item. Would you like to see the price history?


## ❓ FAQ

**Q: Can I search for a customer by their NIF (VAT number) through my agent?**
Yes. Use the `get_customer_by_vat` tool and provide the exact numeric NIF. Your agent will retrieve the certified customer record, ensuring you have the correct fiscal identifiers before generating any new document in Moloni.

**Q: How do I check the internal lines and tax breakdown of an invoice?**
The `get_invoice` tool allows your agent to extract the explicit document body payload. You'll see the individual line items, unit prices, applied tax rates (IVA), and final document totals directly in your conversation.

**Q: Can my agent list all stock movements for a specific product?**
Absolutely. Use the `list_product_stocks` tool with a Product ID. Your agent will report the chronological mutations in your warehouse, helping you audit how inventory levels have changed over time for that specific item.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moloni-cloud-invoicing-fiscal-management](https://vinkius.com/mcp/moloni-cloud-invoicing-fiscal-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moloni (Cloud Invoicing & Fiscal Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moloni-cloud-invoicing-fiscal-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moloni (Cloud Invoicing & Fiscal Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moloni-cloud-invoicing-fiscal-management": {
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

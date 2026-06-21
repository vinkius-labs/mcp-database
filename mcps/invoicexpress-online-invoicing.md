# InvoiceXpress (Online Invoicing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoicexpress-online-invoicing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage invoicing via InvoiceXpress — create clients, track payments, and manage invoices and estimates in Portugal.

## Description
Connect your **InvoiceXpress** account to any AI agent and take full control of your certified invoicing and client management in Portugal through natural conversation.

### What you can do

- **Client Management** — List all registered clients and retrieve detailed fiscal data including NIF/NIPC identifiers, addresses, and contact histories directly from your agent
- **Invoice Lifecycle** — Browse issued invoices and receipts, and access detailed line items and tax breakdowns for each document securely
- **Estimate & Quotes** — List and retrieve estimates and pro-forma invoices to monitor your sales pipeline and pending business proposals
- **Item Inventory** — Manage your catalog of faturable articles and services, including unit prices and associated VAT rates (IVA)
- **Fiscal Compliance** — Audit tax rates and exemptions active in your account to ensure mapping with official AT (Autoridade Tributária) tables
- **Digital Delivery** — Access permalinks to signed PDF documents for easy sharing and visual verification of fiscal items

### How it works

1. Subscribe to this server
2. Enter your InvoiceXpress Account Name and API Key
3. Start managing your certified billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners in Portugal** — monitor outstanding invoices and manage client balances through natural conversation
- **Freelancers & Service Providers** — list and retrieve invoice PDFs for clients without leaving your development or design environment
- **Accounting & Ops Teams** — audit fiscal documents and ensure VAT compliance across the entire invoicing system


## Available Tools
- **list_clients**: Listar todos os clientes registados no InvoiceXpress
- **get_client**: Obter detalhes completos de um cliente pelo seu ID
- **find_client**: Pesquisar um cliente pelo nome empresarial
- **create_client**: Se não for fornecido um NIF, usa o valor Consumer (ou similar requerido pelo portal).

Registar um novo cliente no InvoiceXpress com dados fiscais completos
- **update_client**: Só os parâmetros enviados serão substituídos, os restantes mantêm-se inalterados.

Atualizar os dados demográficos de um cliente existente
- **list_items**: Listar todos os artigos e serviços configurados no InvoiceXpress
- **get_item**: Obter detalhes de um artigo ou serviço pelo seu ID
- **create_item**: Precisas sempre de um ID de taxa legal (consulta a ferramenta list_taxes previamente).

Criar um novo artigo ou serviço para ser faturado
- **list_invoices**: Listar todas as faturas emitidas
- **get_invoice**: Obter todos os detalhes e o link PDF de uma fatura
- **list_estimates**: Listar todos os orçamentos emitidos de forma paginada
- **list_credit_notes**: Listar todas as notas de crédito (devolução / acerto)
- **list_receipts**: Listar todos os recibos de pagamento de clientes
- **list_guides**: Listar guias de transporte
- **list_taxes**: Listar as taxas de IVA e isenções ativas na conta
- **list_sequences**: Listar as séries de faturas ativas, ex: FT 2026/


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InvoiceXpress (Online Invoicing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices from InvoiceXpress"

**🤖 AI Agent:**
> I've retrieved the latest 5 invoices. Highlights include FT 2026/1 (€1,200), FT 2026/2 (€450), and FT 2026/3 (€2,100). All documents are in the 'Finalized' state. Would you like the PDF link for any of these?

---

**👤 You:**
> "Search for a client named 'TechPorto'"

**🤖 AI Agent:**
> I've found client 'TechPorto' (ID: 12345). Their fiscal ID is 500123456 and they are located in Porto. They have 3 active estimates pending approval. Would you like to see their contact history?

---

**👤 You:**
> "What are the active VAT rates in my account?"

**🤖 AI Agent:**
> I've identified 3 active VAT rates: 23% (Normal rate, ID: 1), 13% (Intermediate rate, ID: 2), and 6% (Reduced rate, ID: 3). There are also 2 exemption codes configured for international services. I can provide the IDs for your item mappings.


## ❓ FAQ

**Q: Can I see the signed PDF of an invoice through my agent?**
Yes. Use the `get_invoice` tool with a specific Invoice ID. Your agent will return all document details along with a permalink to the signed PDF, allowing you to view or share the official fiscal document instantly.

**Q: How do I find a client by their company name?**
The `find_client` tool allows you to search for a client directly by their business name. This is perfect for locating a client profile when you don't have their numerical ID handy.

**Q: Can I list the VAT rates available in my account?**
Absolutely. Use the `list_taxes` tool to enumerate all VAT rates and exemptions configured in your InvoiceXpress account. Your agent will show the official AT mapping, which is essential before creating new items or invoices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoicexpress-online-invoicing](https://vinkius.com/mcp/invoicexpress-online-invoicing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **InvoiceXpress (Online Invoicing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `invoicexpress-online-invoicing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **InvoiceXpress (Online Invoicing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoicexpress-online-invoicing": {
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

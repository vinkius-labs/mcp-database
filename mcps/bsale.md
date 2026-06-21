# Bsale MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bsale)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate cloud POS operations via Bsale — issue electronic invoices, manage inventory, track stock levels, and register clients from any AI agent.

## Description
Connect your **Bsale** cloud POS account to any AI agent and take full control of your Chilean retail and invoicing operations through natural conversation.

### What you can do

- **Electronic Document Emission** — Issue SII-compliant boletas, facturas electrónicas, credit notes, and dispatch guides directly through your AI agent
- **Product Catalog Management** — Browse, search, and create products with full variant (SKU) support, pricing tiers, and web descriptions
- **Inventory & Stock Control** — Check real-time stock levels across all office branches and track variant-level availability
- **Client Registry** — Search, inspect, and register customers with RUT, business activity (giro), and contact details for tax compliance
- **Configuration Intelligence** — Query your document types, payment methods, price lists, and office configurations instantly

### How it works

1. Subscribe to this server
2. Enter your Bsale Access Token
3. Start managing your POS from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated retail operations assistant — no more navigating multiple POS screens to issue a simple boleta.

### Who is this for?

- **Retail Store Managers** — issue invoices and check stock without switching between terminals and browsers
- **Accountants** — query document registries and client information for month-end reconciliation
- **E-commerce Operators** — sync product catalogs and manage variant pricing across sales channels


## Available Tools (15)
- **create_client**: The client can then be associated with future invoices and sales documents. For Chilean tax compliance, include the RUT and business activity (giro) when available.

Register a new client in the system
- **create_document**: Requires the document type ID and at minimum one line item with product details. The document is automatically sent to the Chilean SII (Servicio de Impuestos Internos) for validation.

Issue a new electronic tax document
- **create_product**: The product will be available for inclusion in future documents and can be associated with variants (SKUs), price lists, and stock management across multiple offices.

Create a new product in the catalog
- **get_client**: Get full details of a specific client
- **get_document**: Get full details of a specific tax document
- **get_product**: Get full details of a specific product
- **list_clients**: Use limit and offset for pagination.

List all registered clients
- **list_document_types**: List available SII document types
- **list_documents**: Documents are returned with their SII-compliant folio numbers, emission dates, and net/tax/total breakdowns. Use optional limit and offset parameters for pagination.

List tax documents (invoices, boletas, credit notes)
- **list_offices**: List all office branches and locations
- **list_payment_types**: List accepted payment methods
- **list_price_lists**: g., retail, wholesale, distributor). Each price list can have different pricing for the same product variants.

List all configured price lists
- **list_products**: Use limit and offset for paginated browsing of large catalogs.

List all products and services in your catalog
- **list_stocks**: Returns available quantities per location.

Check stock levels across offices
- **list_variants**: Each variant has its own barcode, cost, and pricing configuration across different price lists.

List all SKU variants for a product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bsale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 invoices issued in my Bsale account."

**🤖 AI Agent:**
> I found 10 recent documents. Notable entries include Factura Electrónica #4521 for $128,500 CLP (client: Constructora Andes SpA), Boleta #8903 for $15,900 CLP, and Nota de Crédito #102 voiding document #4518. Would you like the full breakdown of any specific document?

---

**👤 You:**
> "Check stock levels for all variants of product ID 1542."

**🤖 AI Agent:**
> Product 1542 'Zapatilla Running Pro' has 3 variants: Size 40 (SKU: ZRP-40) — 12 units at Santiago Centro, 5 at Providencia. Size 42 (SKU: ZRP-42) — 8 units at Santiago Centro, 0 at Providencia (out of stock!). Size 44 (SKU: ZRP-44) — 3 units at both locations. Should I create a restocking alert?

---

**👤 You:**
> "Register a new client 'Distribuidora Los Andes Ltda' with RUT 76.543.210-K."

**🤖 AI Agent:**
> Client created successfully! 'Distribuidora Los Andes Ltda' has been registered with RUT 76.543.210-K and assigned internal ID #2847. You can now use this client ID when issuing facturas electrónicas or boletas. Would you like to issue an invoice for them right now?


## ❓ FAQ

**Q: Can my AI agent issue a SII-compliant electronic invoice (factura electrónica) directly?**
Yes! Use the `create_document` tool with the appropriate document type ID (factura, boleta, etc.), office ID, and line item details. Bsale automatically validates and transmits the document to Chile's SII for electronic stamping.

**Q: How can I check the stock level of a specific product variant across all my stores?**
Use the `list_stocks` tool with the variant ID as a filter. It will return the current available quantity for that SKU across every office branch configured in your Bsale account, giving you instant cross-store visibility.

**Q: Can I register a new client with their RUT for tax compliance before issuing an invoice?**
Absolutely. Use the `create_client` tool with the client's name, RUT (in the code field), and business activity (giro). Once created, you can immediately reference their client ID when issuing documents through the `create_document` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bsale](https://vinkius.com/mcp/bsale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bsale** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bsale` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bsale** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bsale": {
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

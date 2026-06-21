# Go-UPC MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/go-upc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search products by barcode — audit UPC, EAN, and ISBN via AI.

## Description
Empower your AI agent to orchestrate your entire product discovery and retail auditing workflow with **Go-UPC**, the comprehensive database for barcode data. By connecting Go-UPC to your agent, you transform complex product lookups into a natural conversation. Your agent can instantly retrieve detailed product metadata, audit brand information, and identify categories from any UPC, EAN, or ISBN without you ever touching a manual lookup tool. Whether you are conducting market research or managing inventory, your agent acts as a real-time product specialist, ensuring your retail intelligence is always grounded in accurate, verified data.

### What you can do

- **Product Auditing** — Retrieve high-resolution product details for any UPC or EAN barcode, including descriptions and image links.
- **Brand Oversight** — Identify brand names and manufacturers associated with specific products to maintain a clear view of market distribution.
- **Category Discovery** — Query product categories to understand the organizational hierarchy of your retail data.
- **Bibliographic Intelligence** — Lookup ISBN numbers to retrieve book details and metadata instantly.
- **Operational Monitoring** — Check API status and monitor your lookup history to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your Go-UPC API Key
3. Start managing your product intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Retail Analysts** — monitor product distributions and retrieve competitor metadata straight from your workflow.
- **Inventory Managers** — verify product details and audit barcode accuracy without manual database exports.
- **Researchers** — perform rapid audits of consumer goods and identify brand owners through natural language.
- **Operations Leads** — automate product data querying to orchestrate cross-functional retail teams smoothly.


## Available Tools
- **check_api_status**: Check if the Go-UPC API is operational
- **get_brand_details**: Get information about a specific brand
- **get_category_details**: Get details for a product category
- **get_product_by_code**: Get product details by UPC, EAN, or ISBN barcode
- **search_products**: Search for products by name (Placeholder/Info)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Go-UPC** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for product with UPC 012000000133 using Go-UPC."

**🤖 AI Agent:**
> I've identified that barcode as 'Pepsi Cola 12oz Can'. It belongs to the soft drink category and is manufactured by PepsiCo. Would you like the full product description or image link?

---

**👤 You:**
> "Show details for book with ISBN 9780143127550."

**🤖 AI Agent:**
> I've identified ISBN 9780143127550 as 'The Martian' by Andy Weir. It's published by Penguin Books. I can provide the summary and cover metadata if you'd like.

---

**👤 You:**
> "What brand is associated with barcode 064144030326?"

**🤖 AI Agent:**
> I've retrieved the details. The brand is 'Hunt's' and the product is their 'Classic Tomato Ketchup'. I can assist you with more brand auditing if needed.


## ❓ FAQ

**Q: How do I find my Go-UPC API Key?**
Log in to your [**Go-UPC dashboard**](https://go-upc.com/dashboard), and you will find your API Key under the 'API' section. Copy and paste it below.

**Q: What barcode types are supported?**
Go-UPC supports UPC-A, UPC-E, EAN-8, EAN-13, and ISBN-10/13 barcodes globally.

**Q: Can the agent show product images?**
Yes. The `get_product_by_code` tool retrieves high-quality image URLs where available in the database, allowing your agent to provide visual context.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/go-upc](https://vinkius.com/mcp/go-upc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Go-UPC** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `go-upc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Go-UPC** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "go-upc": {
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

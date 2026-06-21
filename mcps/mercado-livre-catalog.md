# Mercado Livre Catalog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-livre-catalog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create, update, and manage product listings, stock, and prices on Mercado Livre.

## Description
Connect **Mercado Livre Catalog** to any AI agent and streamline your e-commerce operations — manage listings, adjust stock levels, update prices, and discover categories through natural conversation.

### What you can do
- **Create Listings** — Publish new products with full details and attributes
- **Stock Management** — Update inventory levels instantly across all listings
- **Price Updates** — Change prices dynamically to stay competitive
- **Search & Discovery** — Find your active listings and browse categories
- **Attribute Management** — Get mandatory attributes for specific categories (e.g., voltage, size)
- **Deactivation** — Close listings that are no longer available

### How it works
1. Subscribe to this server
2. Enter your Mercado Livre OAuth2 Access Token
3. Start managing your catalog from Claude, Cursor, or any MCP-compatible client

Mercado Livre is the largest e-commerce ecosystem in Latin America.

### Who is this for?
- **E-commerce Sellers** — Keep stock and prices up-to-date without logging into the Seller Panel
- **Inventory Managers** — Automate stock replenishment alerts and updates via AI
- **Digital Marketers** — Quickly publish new campaigns and listings directly from chat


## Available Tools
- **get_domain_attributes**: Get required attributes for a category/domain
- **get_categories**: List top-level categories of Mercado Livre Brasil
- **create_item**: Create a new listing
- **delete_item**: Deactivate a listing (close it)
- **get_item**: Get details of a specific listing
- **update_price**: Update the price of an item
- **search_items**: Note: Full search parameters are available via query string in documentation.

Search for listings belonging to the authenticated user
- **update_stock**: Update available quantity for an item
- **update_item**: Update a listing (title, description, attributes)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Livre Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update the price of item MLB123456 to R$99.90."

**🤖 AI Agent:**
> Price updated successfully! Item is now active at R$99.90.

---

**👤 You:**
> "Create a new listing for a 'Wireless Mouse' in category 'Accessories'."

**🤖 AI Agent:**
> Listing created successfully! ID: MLB789012345. It is now live in the site.

---

**👤 You:**
> "What are the mandatory attributes for the Cellphones category?"

**🤖 AI Agent:**
> Required attributes: Brand, Model, Storage Capacity, Color, Screen Size, RAM.


## ❓ FAQ

**Q: How do I get an Access Token for Mercado Livre?**
Go to the [**Mercado Livre Developers**](https://developers.mercadolivre.com.br) portal, create an App, and use the OAuth2 flow to generate your Access Token. It usually starts with `APP_USR-...`.

**Q: Can I create listings with images?**
Yes, the create_item tool accepts a JSON body where you can include picture IDs. Ensure images are already uploaded to Mercado Livre's servers via their Picture API first.

**Q: How do I update stock for multiple items?**
You can use the update_stock action for each item individually. For bulk updates, we recommend using the stock update endpoint directly or creating a loop in your workflow.

**Q: What listing types does Mercado Livre support?**
Mercado Livre supports several listing types: 'gold_special' (premium with fulfillment), 'gold_pro' (classic), and 'gold' (basic). Each type offers different levels of visibility, fees, and buyer reach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-livre-catalog](https://vinkius.com/mcp/mercado-livre-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mercado Livre Catalog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mercado-livre-catalog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mercado Livre Catalog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mercado-livre-catalog": {
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

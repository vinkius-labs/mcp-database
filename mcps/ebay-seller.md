# eBay Seller MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebay-seller)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect eBay Seller to any AI agent via MCP.



## Available Tools
- **get_account_info**: Use this to verify account status or display seller metrics.

Get your eBay seller account information and feedback score
- **create_listing**: Requires SKU (from inventory), listing title, category ID, pricing, format (FIXED_PRICE or AUCTION), and return/shipping policies. Returns listingId for management. Use this to make your inventory products visible to buyers.

Create a new eBay listing for an inventory item
- **delete_inventory**: Note: you cannot delete inventory items that have active listings. Use this to clean up discontinued products.

Delete an inventory item by SKU
- **delete_listing**: If there are active bids (auction), this may violate eBay policies. For fixed-price, this simply removes the item from sale. Use this to quickly remove unwanted inventory from the marketplace.

Delete/end an eBay listing
- **get_inventory_item**: Use this to verify product details before updating or creating listings.

Get detailed information for a specific inventory item by SKU
- **get_orders**: Optional filter parameter accepts criteria like "creationDate:[2024-01-01..2024-12-31]", "orderFulfillmentStatus:NOT_STARTED". Use this to manage order fulfillment pipeline.

List recent orders with optional filtering
- **list_inventory**: Each item includes SKU, title, condition, and available quantity. Use optional limit (default 50) and offset for pagination. Essential for reviewing stock levels.

List all inventory items with SKUs, titles, and available quantities
- **list_listings**: Each listing includes title, price, status, listing ID, and associated SKU. Use this to review what is currently live on eBay or recently ended.

List active eBay listings for your store
- **get_order_details**: Use this to verify order contents before packing and shipping.

Get detailed information for a specific order
- **ship_order**: Updates buyer with shipping notification. Requires orderId, lineItemId, carrier name (e.g., "USPS", "FedEx", "UPS"), and tracking number. Use this to confirm shipment and complete the order cycle.

Mark an order as shipped with carrier and tracking number
- **update_inventory**: Requires SKU, title, condition, and product details (brand, MPN, UPC/EAN, description). Also updates stock quantity and pricing. Use this to manage your product catalog before listing items for sale.

Update or create an inventory item with product details and stock quantity
- **update_listing**: Note: certain fields cannot be changed once listing is active. Use this to adjust pricing or correct listing errors.

Update an existing eBay listing (price, title, details)






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebay-seller](https://vinkius.com/mcp/ebay-seller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eBay Seller** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ebay-seller` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eBay Seller** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebay-seller": {
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

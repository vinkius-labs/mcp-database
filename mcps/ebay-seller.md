# eBay Seller MCP Server

Connect eBay Seller to any AI agent via MCP.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ebay-seller)

## Overview
**Category:** industry-titans
**Tools Count:** 12



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

To install and use the **eBay Seller** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebay-seller](https://vinkius.com/mcp/ebay-seller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

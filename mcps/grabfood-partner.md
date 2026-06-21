# GrabFood Partner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grabfood-partner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate GrabFood restaurant operations — manage orders, update menus, control store status, and run marketing campaigns directly from any AI agent.

## Description
Connect your **GrabFood Partner** account to any AI agent and take full control of your restaurant delivery operations through natural conversation.

### What you can do

- **Order Management** — List all incoming orders, accept or reject them, cancel when necessary, and mark orders as ready for pickup
- **Order Lifecycle Control** — Check if orders can be cancelled, update estimated ready times, and manage delivery states
- **Menu Management** — Update your entire menu or perform targeted batch updates to specific items, prices, and availability
- **Store Operations** — Check your store's real-time status, view operating hours, and pause/unpause your store instantly
- **Marketing Campaigns** — List existing campaigns and create new promotional campaigns to boost visibility and orders

### How it works

1. Subscribe to this server
2. Enter your GrabFood Partner OAuth2 access token
3. Start managing your GrabFood restaurant from Claude, Cursor, or any MCP-compatible client

No more logging into the partner portal during a lunch rush. Your AI acts as an instant operations assistant for your GrabFood delivery business.

### Who is this for?

- **Restaurant Owners** — manage orders and menus hands-free while working in the kitchen
- **Operations Managers** — monitor multiple GrabFood locations, check statuses, and adjust availability on the fly
- **Marketing Teams** — launch and track promotional campaigns without navigating the partner dashboard


## Available Tools
- **accept_order**: This is a critical operational tool for restaurant staff to manage order flow. When set to accept=true, the restaurant confirms it will prepare the order. When accept=false, the order is rejected and the customer is notified.

**Parameters:**
- `order_id` (required): The unique order ID from GrabFood that needs to be accepted or rejected.
- `accept` (required): Boolean flag — true to accept the order, false to reject it.

**When to use:**
- User says "accept order 12345" to confirm they will prepare it
- User says "reject order 12345" if the restaurant cannot fulfill the order (e.g., items out of stock, kitchen closed)
- User wants to bulk-accept multiple orders during busy periods
- User needs to decline an order due to operational constraints

**Important:** Accepting an order commits the restaurant to preparing it. Rejecting may impact the merchant's performance metrics on the GrabFood platform. Always verify order details before accepting.

Accept or reject a GrabFood order
- **batch_update_menu**: This is the preferred tool for making incremental changes — such as updating prices for a few items, marking items as available/unavailable, or modifying descriptions.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.
- `items` (required): An array of item update objects. Each object should contain the item identifier and the fields to update (e.g., price, availability, name, description).

**When to use:**
- User needs to update prices for only a subset of menu items
- User wants to mark several items as sold out without touching the full menu
- User wants to update descriptions or names for specific dishes
- Incremental daily changes (e.g., "mark items X, Y, Z as unavailable today")
- User wants to avoid the risk of a full menu replacement

**Important:** This is safer than a full menu update because it only touches the items you specify. Each item in the batch should include its identifier (e.g., item_id or sku) and only the fields that need changing.

Batch update specific menu items for a GrabFood merchant
- **cancel_order**: This should be used sparingly as cancellations negatively impact the merchant's performance score on GrabFood. Always verify the order can be cancelled before attempting.

**Parameters:**
- `order_id` (required): The unique order ID of the order to cancel.
- `reason` (optional): A brief explanation for why the order is being cancelled. Providing a reason is recommended for audit purposes (e.g., "item out of stock", "kitchen equipment failure", "customer request").

**When to use:**
- User discovers an item is out of stock after accepting an order
- User needs to cancel due to unforeseen kitchen issues
- Customer has requested a cancellation
- Duplicate order was accidentally accepted

**Important:** Before cancelling, consider using `check_order_cancelable` to verify if the order is still in a cancellable state. Once the order has progressed too far in preparation, cancellation may not be possible.

Cancel an already accepted GrabFood order
- **check_order_cancelable**: This is a safety check tool that should be used before attempting to cancel an order, as cancellations after a certain point in the order lifecycle are not permitted.

**Parameters:**
- `order_id` (required): The unique order ID to check for cancellation eligibility.

**When to use:**
- Before cancelling an order to avoid API errors
- User asks "can I still cancel order 12345?"
- Restaurant staff needs to verify order state before making a cancellation decision
- User is uncertain whether the order has progressed beyond the cancellation window

**Returns:** A status object indicating whether the order can be cancelled, along with any relevant state information.

Check if a GrabFood order can still be cancelled
- **create_campaign**: Campaigns can include discounts, free delivery offers, featured placement, and other promotional tools designed to increase order volume and visibility.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.
- `campaign` (required): The campaign configuration as a JSON object. This typically includes campaign name, type (e.g., discount, free delivery), budget, start/end dates, target audience, and any specific promotional parameters.

**When to use:**
- User wants to launch a promotional discount to boost order volume
- User needs to set up a free delivery campaign for a limited period
- Restaurant is opening a new location and wants featured placement
- User wants to run a time-limited promotional offer (e.g., "20% off this weekend")

**Important:** Campaign creation may require budget approval from GrabFood. Ensure the campaign configuration matches GrabFood's accepted campaign types and schemas. Review campaign details carefully before submitting, as changes may not be possible after creation.

Create a new marketing campaign for a GrabFood merchant
- **get_store_status**: This includes whether the store is currently open, paused, or closed, along with any status flags that affect order acceptance.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.

**When to use:**
- User asks "is my store currently open on GrabFood?"
- User wants to verify the store's visibility to customers
- Before opening or closing, to check the current state
- User wants to troubleshoot why orders are not coming in
- User needs to audit store operational status

**Returns:** A status object containing the store's current state (open/closed/paused), any active flags, and potentially operational metadata like current order capacity.

Get the current operational status of a GrabFood store
- **list_campaigns**: Campaigns on GrabFood are used to promote the restaurant through discounts, free delivery, featured placement, and other marketing initiatives.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.

**When to use:**
- User asks "what campaigns am I currently running on GrabFood?"
- User wants to review the performance of past marketing campaigns
- User needs to see active promotions before creating a new one
- User wants to audit their marketing spend on GrabFood

**Returns:** A JSON array of campaign objects, each containing campaign details such as name, type, budget, duration, status, and performance metrics.

List all marketing campaigns for a GrabFood merchant
- **list_orders**: Use this tool when the user wants to see what orders have been placed, check today's order volume, or review incoming orders from GrabFood delivery customers.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood Partner Portal. This identifies which restaurant's orders to fetch.
- `date` (optional): The date to filter orders by, in YYYY-MM-DD format. If not provided, the API returns the most recent orders.

**When to use:**
- User asks "what orders do I have today?"
- User wants to check order history for a specific date
- User needs to see all incoming GrabFood orders before accepting them
- User wants to audit order volume for a given day

**Returns:** A JSON array of order objects, each containing order_id, items, customer details, delivery information, and order status.

List all GrabFood orders for a merchant on a specific date
- **mark_order_ready**: This is a crucial step in the order lifecycle — it notifies Grab that the driver should arrive immediately.

**Parameters:**
- `order_id` (required): The unique order ID that has been prepared and is ready for collection.

**When to use:**
- Kitchen has finished preparing all items in the order
- User says "order 12345 is ready for pickup"
- User wants to notify Grab that the driver should come now
- All items have been packed and verified against the order

**Important:** Only mark an order as ready when it is genuinely complete. Premature marking causes driver arrival before food is ready, leading to poor customer experience and potential quality issues (cold food, etc.).

Mark a GrabFood order as ready for pickup/delivery
- **pause_store**: When paused, the store will not receive new orders from GrabFood customers. When unpaused (pause=false), the store becomes visible and active again.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.
- `pause` (required): Boolean flag — true to pause the store, false to unpause it.

**When to use:**
- User says "pause my GrabFood store" — e.g., kitchen is overwhelmed, staff shortage, or end of business day
- User says "unpause my store" or "open my store" when ready to receive orders again
- Emergency closure due to equipment failure, power outage, or other disruptions
- User wants to temporarily stop accepting orders during a rush

**Important:** Pausing the store immediately stops new orders from being placed. Existing active orders are not affected. Always verify the store status after pausing/unpausing using `get_store_status` to confirm the change took effect.

Pause or unpause a GrabFood store
- **update_menu**: This tool replaces or modifies menu items, categories, pricing, and availability. It is a full update operation — ensure all desired menu data is included in the payload.

**Parameters:**
- `merchant_id` (required): The unique merchant ID registered with GrabFood.
- `menu` (required): The complete menu data structure to update. This typically includes categories, items, prices, descriptions, images, and availability flags. The exact structure depends on the GrabFood menu schema.

**When to use:**
- User wants to add new dishes or remove discontinued items
- User needs to update prices across the menu
- Restaurant is changing its operating menu (e.g., seasonal items)
- User needs to mark certain items as unavailable temporarily
- User wants to update item descriptions or images

**Important:** This is a full update operation. If you need to update only specific items without affecting the rest of the menu, consider using `batch_update_menu` instead. Ensure the menu data structure matches GrabFood's expected schema to avoid rejection.

Update the menu for a GrabFood merchant
- **update_ready_time**: This helps Grab optimize driver dispatch timing so the driver arrives when the food is actually ready, not too early or too late.

**Parameters:**
- `order_id` (required): The unique order ID whose ready time needs updating.
- `ready_time` (required): The new estimated ready time in ISO 8601 format (e.g., "2024-01-15T14:30:00+07:00"). This should be a future timestamp representing when the order will be ready.

**When to use:**
- Kitchen is running behind schedule and the original estimate is no longer accurate
- User wants to push back the ready time due to high order volume
- Complex items are taking longer than expected to prepare
- User wants to proactively manage driver dispatch timing

**Important:** The ready_time should be in ISO 8601 format with timezone. Updating this too frequently or with unrealistic times may impact merchant performance ratings.

Update the estimated ready time for a GrabFood order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GrabFood Partner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my GrabFood orders for today."

**🤖 AI Agent:**
> I've fetched your GrabFood orders for today. You currently have 8 active orders, with 3 pending acceptance and 5 being prepared. The most recent order (#GF-48921) includes 2x Nasi Goreng and 1x Es Teh Manis. Would you like to accept all pending orders?

---

**👤 You:**
> "Accept order GF-48921 and mark order GF-48915 as ready."

**🤖 AI Agent:**
> Done! Order GF-48921 has been accepted and the kitchen can now start preparing it. Order GF-48915 has been marked as ready for pickup — the Grab driver will be notified to arrive shortly.

---

**👤 You:**
> "Check my store status and pause it if it's currently open."

**🤖 AI Agent:**
> Your GrabFood store is currently **open** and accepting orders. I've paused it for you — the store is now hidden from customers and no new orders will come through. Existing active orders are unaffected.

---

**👤 You:**
> "Update the price of my Nasi Goreng to 25000 IDR and mark Fried Rice as unavailable."

**🤖 AI Agent:**
> I've batch-updated your menu: Nasi Goreng price is now 25,000 IDR and Fried Rice has been marked as unavailable. Customers will see these changes reflected on the GrabFood app within a few minutes.


## ❓ FAQ

**Q: How do I get my GrabFood Merchant ID?**
Your Merchant ID is provided when you register as a GrabFood Partner. You can find it in the GrabFood Partner Portal under your restaurant settings, or in the welcome email you received when your restaurant was onboarded to GrabFood.

**Q: Can I use this integration in production, not just sandbox?**
Yes! The integration defaults to the GrabFood sandbox environment for safe testing. To switch to production, you'll need to update the base URL in the engine configuration to the production endpoint. Contact GrabFood Partner support for production API credentials.

**Q: What happens if I reject an order? Does it affect my merchant rating?**
Rejecting orders may impact your merchant performance metrics on GrabFood. Frequent rejections can lead to lower visibility in search results. It's recommended to only reject orders when absolutely necessary (e.g., item out of stock, kitchen closure). Always verify order details before making a decision.

**Q: Can I update menu items individually without replacing the entire menu?**
Yes! Use the `batch_update_menu` tool for targeted updates to specific items, prices, or availability. This is safer than a full menu replacement since it only touches the items you specify. Use `update_menu` only when you need to replace the entire menu structure.

**Q: How do I get my OAuth2 access token for the GrabFood Partner API?**
You can obtain your OAuth2 access token through the GrabFood Partner Portal. Log in to your partner account and navigate to API Settings or Developer section to generate or retrieve your token. If you don't have access, contact your GrabFood Partner account manager.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grabfood-partner](https://vinkius.com/mcp/grabfood-partner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GrabFood Partner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grabfood-partner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GrabFood Partner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grabfood-partner": {
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

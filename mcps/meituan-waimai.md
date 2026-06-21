# Meituan Waimai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meituan-waimai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Essential food delivery gig API — manage orders, track delivery, handle refunds, and control restaurant menus via Meituan Waimai.

## Description
Connect your **Meituan Waimai (美团外卖)** restaurant operations to any AI agent and transform your delivery management through natural conversation. Meituan Waimai is China's largest food delivery platform, handling millions of daily orders across hundreds of thousands of restaurants.

### What you can do

- **Order Management** — Retrieve detailed order information, list orders by status (pending, confirmed, delivering, completed, cancelled)
- **Order Lifecycle Control** — Confirm new orders, mark orders as delivering, complete deliveries, or cancel with explanations
- **Refund Processing** — Approve or reject customer refund requests with detailed reasoning and order verification
- **Restaurant Information** — Query restaurant details including ratings, addresses, business hours, and delivery coverage
- **Menu Management** — List full restaurant catalogs, filter by category, view prices, descriptions, and stock levels
- **Stock Control** — Update item availability in real-time, mark items as sold out, or replenish inventory
- **Delivery Tracking** — Mark orders as out for delivery with rider information for customer transparency

### How it works

1. Subscribe to this server
2. Enter your Meituan Waimai App ID and App Secret
3. Start managing your restaurant operations from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your restaurant operations manager, handling order confirmations, monitoring stock levels, processing refunds, and optimizing your menu — all through conversational commands.

### Who is this for?

- **Restaurant Owners** — Monitor incoming orders, manage menus, and handle refunds without logging into the merchant dashboard
- **Multi-Location Operators** — Query order volumes and restaurant info across multiple POIs from a single AI interface
- **Kitchen Staff** — Check order details, confirm new orders, and mark items as sold out when ingredients run low
- **Customer Service** — Track order status, investigate refund claims, and resolve delivery issues quickly


## Available Tools
- **cancel_order**: Requires a cancellation reason explaining why the order is being cancelled (e.g., "restaurant closed", "item out of stock", "unable to prepare"). The order must be in a cancellable state (not already completed or delivered). Use carefully as cancellations impact merchant ratings and customer experience.

Cancel a Meituan delivery order with a reason
- **complete_order**: This is the final state in the order lifecycle and indicates the customer has received their food. Should only be called after the delivery rider has confirmed drop-off or the customer has picked up the order. Triggers payment settlement to the merchant.

Mark a Meituan delivery order as completed
- **confirm_order**: This transitions the order to confirmed status and begins the preparation workflow. Required step before marking the order as delivering. Use the order ID from the order list and the restaurant POI ID. Essential for acknowledging new orders and starting the fulfillment process.

Confirm a pending Meituan delivery order
- **get_order_detail**: Use the order ID obtained from the order list to track specific orders, verify order contents, check delivery addresses, or investigate customer complaints. Essential for order management and customer service operations.

Get detailed information about a specific Meituan delivery order
- **get_order_list**: Filter by order status: 1=待确认 (pending confirmation), 3=已确认 (confirmed), 5=配送中 (delivering), 7=已完成 (completed), 8=已取消 (cancelled). Pagination uses page number and limit parameters. Critical for monitoring incoming orders, tracking order volume, and managing the order pipeline.

List orders for a Meituan restaurant with optional status filter
- **get_restaurant_info**: Use the POI ID (Point of Interest identifier) to get restaurant details before managing orders, verifying delivery coverage, or checking business hours. Essential for multi-restaurant operators managing multiple POIs.

Get detailed information about a Meituan restaurant/POI
- **handle_refund**: When rejecting, provide a reason explaining the refusal. Refund requests typically come with customer explanations and evidence. Use order details to verify the claim before making a decision. Approved refunds are processed back to the customer's original payment method.

Approve or reject a refund request for a Meituan order
- **list_menus**: Optionally filter by category ID to get items from a specific menu section (e.g., appetizers, mains, drinks). Critical for inventory management, price updates, and menu optimization. Returns stock quantities to help identify low-stock items.

List menu items for a Meituan restaurant
- **mark_delivering**: Optionally includes delivery rider name and phone number for customer tracking. Use this for self-delivery orders where the restaurant manages their own riders. For Meituan-managed delivery, the platform handles this automatically.

Mark a Meituan order as being delivered (out for delivery)
- **update_stock**: Use this to mark items as sold out (stock=0) when ingredients run out, or replenish stock when new inventory arrives. Stock changes immediately reflect on the customer-facing menu. Essential for preventing orders for unavailable items and maintaining accurate inventory. Food ID is obtained from the list_menus tool.

Update stock quantity for a menu item in Meituan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meituan Waimai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending orders for my restaurant POI123."

**🤖 AI Agent:**
> 📋 Found 3 pending orders for POI123: Order #ORD-001 (¥45.50, 2 items, customer: Zhang Wei), Order #ORD-002 (¥78.00, 4 items, customer: Li Na), Order #ORD-003 (¥32.00, 1 item, customer: Wang Fang). All orders are awaiting your confirmation. Would you like me to confirm all of them?

---

**👤 You:**
> "Mark food ID 4567 as sold out for POI123 — we ran out of chicken."

**🤖 AI Agent:**
> ✅ Stock updated successfully! Food item #4567 has been marked as sold out (stock=0) for restaurant POI123. The item is no longer visible on the customer menu, preventing new orders until you replenish stock.

---

**👤 You:**
> "Handle refund request for order ORD-789 — customer says food never arrived. Approve it."

**🤖 AI Agent:**
> ✅ Refund approved and processed successfully! Order ORD-789 refund has been approved. The refund amount (¥56.00) will be returned to the customer's original payment method within 1-3 business days. The customer has been notified of the successful refund.


## ❓ FAQ

**Q: How do I get my Meituan Waimai App ID and App Secret?**
Log in to the [Meituan Waimai Developer Console](https://developer.waimai.meituan.com/), navigate to **API Documentation** > **Access Guide**, and register your application. You'll receive an App ID and App Secret. Make sure your application has the required API permissions for order management, menu access, and refund handling. The signature algorithm uses MD5 hashing of sorted parameters combined with your App Secret.

**Q: What's the order lifecycle in Meituan Waimai?**
The typical order flow is: **1) Pending (待确认, status=1)** — Customer placed order, awaiting merchant confirmation. **2) Confirmed (已确认, status=3)** — Merchant accepted the order, kitchen starts preparation. **3) Delivering (配送中, status=5)** — Food is out for delivery with rider. **4) Completed (已完成, status=7)** — Customer received the order, payment settled. **5) Cancelled (已取消, status=8)** — Order was cancelled by merchant or customer. At each stage, you can query details, and merchants can confirm, mark delivering, or complete the order.

**Q: How do I handle stock management and sold-out items?**
Use the `update_stock` tool to set stock quantities for menu items. Set `stock=0` to mark an item as sold out (it will immediately disappear from the customer menu). Set a positive number to replenish stock. Get the food ID from the `list_menus` tool first. This is critical during peak hours when ingredients run out — quickly updating stock prevents customers from ordering unavailable items and reduces refund requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meituan-waimai](https://vinkius.com/mcp/meituan-waimai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meituan Waimai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meituan-waimai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meituan Waimai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meituan-waimai": {
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

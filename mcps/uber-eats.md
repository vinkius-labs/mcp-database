# Uber Eats MCP Server

AI restaurant management: manage orders, menus, deliveries, and store operations via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/uber-eats)

## Overview
**Category:** industry-titans
**Tools Count:** 14

## Description
### What you can do

Connect AI agents to the Uber Eats Marketplace API for complete restaurant and delivery management:

- **Monitor incoming orders** in real-time with status tracking (PENDING → ACCEPTED → PREPARING → READY → DELIVERED)
- **Accept or reject orders** instantly based on kitchen capacity
- **Manage restaurant menus** — update prices, availability, descriptions, dietary tags
- **Review order details** including customer info, items, special instructions, and totals
- **Track delivery status** with real-time courier GPS location and ETA
- **Handle order issues** including customer complaints and refund requests
- **View store information** and configuration across all registered locations
- **Mark orders ready** for courier pickup when food is prepared

### How it works

1. **Connect your Uber Eats merchant account** via OAuth token from Uber Developer Portal
2. **Ask your AI agent** to check orders, update menus, track deliveries, or manage stores
3. **Natural language commands** replace manual Uber Eats Manager app navigation
4. **Automate repetitive tasks** like accepting orders, updating availability, and tracking deliveries

### Who is this for?

Essential for **restaurant owners**, **food delivery managers**, **multi-location food businesses**, **ghost kitchen operators**, **franchise managers**, and **POS system integrators** using Uber Eats. Let AI agents handle order monitoring, menu maintenance, delivery tracking, and store management. Perfect for businesses processing 20+ daily orders who want faster response times, reduced manual oversight, and streamlined operations across multiple restaurant locations.


## Available Tools
- **accept_order**: This notifies the customer that the restaurant is preparing their food and triggers courier assignment by Uber Eats. Required before marking order as ready for pickup. Use this to acknowledge incoming orders and begin food preparation. Should be done promptly to maintain good restaurant ratings.

Accept a pending Uber Eats order to confirm preparation
- **cancel_order**: This is different from rejection - cancellation happens after acceptance and may result in customer dissatisfaction and potential platform penalties. Requires a cancellation reason. Use only when absolutely necessary (kitchen emergency, safety issue, or unavoidable circumstance).

Cancel an already accepted Uber Eats order
- **complete_order**: This should be called after confirmation that the delivery was successful. Closes the order lifecycle and triggers final payment processing. Use this to confirm order completion.

Mark an order as fully completed (delivered and finalized)
- **get_delivery_status**: Use this to track delivery progress, answer customer inquiries about their order, or coordinate with couriers.

Get real-time delivery tracking status for an Uber Eats order
- **get_menus**: Use this to review menu structure, check which items are available/out of stock, or get menu item IDs needed for availability updates.

Get complete menu catalog for a specific Uber Eats restaurant
- **get_order_issues**: Returns issue descriptions, timestamps, resolution status, and any refunds issued. Use this to review and address order problems, improve quality, and handle disputes proactively.

Get reported issues and complaints for a specific Uber Eats order
- **get_order**: Use this to review order contents before accepting, verify special instructions, or prepare items correctly.

Get complete details of a specific Uber Eats delivery order
- **get_orders**: Can filter by status: PENDING (awaiting restaurant acceptance), ACCEPTED (restaurant confirmed), PREPARING (food being prepared), READY (ready for courier pickup), DELIVERED (completed), CANCELLED, or REJECTED. Returns order IDs, customer info, items ordered, totals, special instructions, and timestamps. Use this to monitor order flow, track pending orders requiring action, or review completed deliveries.

List all orders for your Uber Eats restaurants with optional status filter
- **get_store**: Use this to review store configuration, verify delivery settings, or check operational status.

Get detailed information about a specific Uber Eats restaurant/store
- **get_stores**: Returns external store IDs, names, addresses, operating status, and business details. Use this tool first to get your store IDs, which are required for all other menu and order management operations.

List all restaurants/stores associated with your Uber Eats merchant account
- **mark_order_prep_started**: Updates order status to PREPARING and notifies the customer. Use this to keep customers informed about their order progress and provide accurate delivery time estimates.

Mark that food preparation has started for an accepted order
- **mark_order_ready**: This triggers courier dispatch notification. Use this when food is complete and waiting for courier arrival. Couriers will be routed to your location for pickup.

Mark order as ready for courier pickup (food is packaged and waiting)
- **reject_order**: The customer is notified and refunded automatically. Provide a reason code: "item_unavailable" (key ingredients out of stock), "too_busy" (kitchen at capacity), "kitchen_closed" (outside operating hours), or "other". Use this when unable to fulfill an order. Excessive rejections may affect restaurant visibility on the platform.

Reject a pending Uber Eats order when unable to fulfill it
- **update_menu_item_availability**: Set available=true to mark item as in-stock and orderable, or available=false to mark as out-of-stock. Common use: quickly mark items as unavailable when ingredients run out, then re-enable when restocked. Requires external store ID and menu item ID from get_menus result.

Toggle availability status of a menu item (mark as in-stock or out-of-stock)


## Installation & Usage

To install and use the **Uber Eats** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uber-eats](https://vinkius.com/mcp/uber-eats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

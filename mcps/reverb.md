# Reverb MCP Server

Manage your Reverb shop — create listings, track orders, handle payouts, and communicate with buyers directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reverb)

## Overview
**Category:** ecommerce
**Tools Count:** 30

## Description
Connect your **Reverb** seller account to any AI agent to manage your musical gear marketplace operations through natural conversation.

### What you can do

- **Listing Management** — Create, update, publish, or end listings and manage drafts efficiently using `create_listing` and `list_drafts`.
- **Order Fulfillment** — Retrieve orders, mark them as shipped or picked up, and track your seller sales with `retrieve_orders` and `ship_order`.
- **Financial Insights** — Access payment methods, list payouts, and inspect specific payout line items via `list_payouts`.
- **Customer Engagement** — List conversations, reply to buyers, and manage feedback received or sent using `reply_to_conversation`.
- **Shop Operations** — Toggle vacation mode and check your shop's current status with `get_vacation_status`.

### How it works

1. Subscribe to this server
2. Enter your Reverb Personal Access Token
3. Start managing your gear shop from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Gear Sellers** — quickly update prices or end listings without navigating the web interface
- **Shop Managers** — handle customer inquiries and order shipping statuses directly from your workflow
- **Power Users** — automate reporting on payouts and sales performance


## Available Tools
- **add_to_sale**: Add listings to a sale
- **bump_listing**: Bump a listing
- **create_listing**: Requires a JSON payload matching Reverb listing schema.

Create a new Reverb listing
- **delete_draft**: Delete a draft listing
- **delete_listing_image**: Delete an image from a listing
- **disable_vacation_mode**: Disable vacation mode for the shop
- **enable_vacation_mode**: Enable vacation mode for the shop
- **end_listing**: End an active Reverb listing
- **find_listings**: Can filter by SKU or state.

Find seller listings
- **get_bump_info**: Get bump info for a listing
- **get_feedback_received**: Get received feedback
- **get_feedback_sent**: Get sent feedback
- **get_listing_images**: Find image IDs for a listing
- **get_order_payment**: Get payment information for an order
- **get_payment_methods**: Get eligible payment methods
- **get_payout_line_items**: Get line items for a payout
- **get_vacation_status**: Get vacation mode status
- **leave_feedback**: Leave feedback for a buyer
- **list_conversations**: List messages and conversations
- **list_drafts**: List all draft listings
- **list_payouts**: List earnings payouts
- **mark_order_picked_up**: Mark an order as picked up
- **publish_listing**: Publish a draft Reverb listing
- **remove_bump**: Remove a bump from a listing
- **remove_from_sale**: Remove listings from a sale
- **reply_to_conversation**: Reply to a conversation
- **retrieve_orders**: Retrieve selling orders
- **ship_order**: Mark an order as shipped
- **update_listing**: Update an existing Reverb listing
- **view_seller_sales**: View seller sales


## Installation & Usage

To install and use the **Reverb** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reverb](https://vinkius.com/mcp/reverb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

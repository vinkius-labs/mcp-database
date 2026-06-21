# Reverb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reverb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Reverb shop — create listings, track orders, handle payouts, and communicate with buyers directly via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reverb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all my active listings with the SKU 'GUITAR-001'."

**🤖 AI Agent:**
> I'm searching your listings... I found one active listing for 'GUITAR-001': a 1965 Vintage Stratocaster priced at $4,500. Would you like to see the full details or images?

---

**👤 You:**
> "Check if my shop is currently in vacation mode."

**🤖 AI Agent:**
> Checking your shop status... Your shop is currently active and NOT in vacation mode. You can use `enable_vacation_mode` if you need to take a break.

---

**👤 You:**
> "List my recent payouts and their amounts."

**🤖 AI Agent:**
> Retrieving your payout history... I found 3 recent payouts: $120.50 on May 10th, $450.00 on May 12th, and $89.00 on May 15th. Do you want to see the line items for any of these?


## ❓ FAQ

**Q: Can I see my unpublished listings or drafts?**
Yes, you can use the `list_drafts` tool to retrieve all listings that are currently in draft state but not yet live on the marketplace.

**Q: How do I update the shipping status of a sold item?**
Use the `ship_order` tool. You will need to provide the order ID and relevant shipping details to mark the transaction as fulfilled.

**Q: Is it possible to reply to buyer messages directly?**
Absolutely. Use `list_conversations` to find the thread and `reply_to_conversation` to send your message back to the buyer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reverb](https://vinkius.com/mcp/reverb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reverb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `reverb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reverb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reverb": {
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

# Square MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/square-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage payments, customers, and inventory on Square with AI agents.

## Description
Connect your **Square** account to any AI agent to automate your omnichannel commerce and business management. Square provides a robust suite of APIs for processing payments, managing customer relationships, and tracking inventory across all your physical and digital locations through natural conversation.

### What you can do

- **Payment & Transaction Orchestration** — List recent payments and retrieve detailed metadata for specific transactions to ensure your revenue is always synchronized.
- **Customer CRM Control** — List and search through your customer database and manage profile metadata directly from the AI interface.
- **Order Lifecycle Management** — Search and monitor orders across your account to maintain a clear overview of your sales performance.
- **Inventory & Stock Tracking** — Retrieve real-time inventory counts for catalog objects to ensure your product availability is always accurate.
- **Location Oversight** — Access and monitor all business locations and their associated metadata via natural language commands.

### How it works

1. Subscribe to this server
2. Enter your Square Personal Access Token from your developer dashboard
3. Start managing your commerce operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners & Retailers** — quickly check recent sales and inventory levels without switching apps.
- **Customer Success Teams** — automate the retrieval of customer order history and profile details via natural conversation.
- **Operations Managers** — streamline the monitoring of multi-location data and track payment statuses directly within the chat.


## Available Tools (11)
- **create_payment**: Create a new payment
- **get_customer**: Get details for a specific customer
- **list_catalog**: List all catalog items
- **get_stock_count**: Retrieve stock levels
- **get_order_details**: Get metadata for an order
- **get_payment_details**: Get metadata for a payment
- **list_customers**: List store customers
- **list_store_locations**: List your business locations
- **list_payments**: Supports pagination.

List recent store payments
- **search_customers**: Search for specific customers
- **search_orders**: Requires location_ids.

Search for store orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Square** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active business locations in my Square account."

**🤖 AI Agent:**
> I've retrieved your locations. You have 3 active ones: 'Main Street Boutique', 'Downtown Café', and 'Online Store'. Which one would you like to check inventory for?

---

**👤 You:**
> "Show me all payments from today with their status, amounts, and payment methods."

**🤖 AI Agent:**
> 67 payments today totaling $12,340. Completed (62): $11,890. Pending (3): $340. Failed (2): $110 (insufficient funds). By method: Credit card (45, $8,900), Apple Pay (12, $2,100), Cash (8, $980), Gift card (2, $360). Average transaction: $184.18. Largest: $890 (order #SQ-4523). By location: "Downtown Store" (34 payments, $6,200), "Mall Kiosk" (23, $4,100), "Online" (10, $2,040). Tips collected: $456. Refunds processed: 2 ($89 total).

---

**👤 You:**
> "Search for all orders from customer David Chen and show his purchase history."

**🤖 AI Agent:**
> Customer: David Chen (ID: cust_abc123). Member since: March 2024. Total orders: 23. Lifetime value: $4,567. Last order: May 14 (order #SQ-4501, $234, 3 items). Favorite items: "Espresso Blend" (ordered 12 times), "Ceramic Mug" (3 times). Average order: $198.57. Payment methods on file: Visa ending 4521, Apple Pay. Loyalty points: 2,340. Rewards redeemed: 4 ($120 total). Last visit: Downtown Store (2 days ago). Preferred location: Downtown Store (18 of 23 orders).


## ❓ FAQ

**Q: How do I find my Square Personal Access Token?**
Log in to your [**Square Developer Dashboard**](https://developer.squareup.com/apps), create or select an application, and you will find your Personal Access Token in the **Credentials** section. Ensure you use the Production token for live data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/square-alternative](https://vinkius.com/mcp/square-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Square** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `square-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Square** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "square-alternative": {
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

# Smeetz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smeetz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Smeetz commerce operations — list products, handle bookings, and manage customer data directly from any AI agent.

## Description
Connect your **Smeetz** account to any AI agent to streamline your booking and commerce workflows through natural conversation.

### What you can do

- **Product Catalog** — List all available products in your account and fetch detailed metadata for specific items using their unique IDs.
- **Booking Management** — Create new bookings for specific products and dates, including ticket details and customer information, or retrieve existing booking statuses.
- **Customer Insights** — Access your full customer list and retrieve detailed profiles to provide personalized service or analyze buyer behavior.
- **Real-time Queries** — Get instant information on product availability and booking details without leaving your AI interface.

### How it works

1. Subscribe to this server
2. Enter your Smeetz API Key
3. Start managing your commerce operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly check product details and booking statuses without navigating the Smeetz dashboard.
- **Customer Support Teams** — retrieve customer profiles and booking information instantly to resolve inquiries faster.
- **Sales Teams** — create bookings on the fly during customer interactions.


## Available Tools
- **create_booking**: Requires product ID, date, ticket details, and customer information.

Create a new booking for a specific product and date
- **list_customers**: List all customers
- **get_booking**: Get detailed information about a specific booking
- **get_customer**: Get detailed information about a specific customer
- **get_product**: Get detailed information about a specific product
- **list_products**: List all products available in your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smeetz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products available in my Smeetz account."

**🤖 AI Agent:**
> I've retrieved your products. You have 'Grand Canyon Helicopter Tour' (ID: 789) and 'Las Vegas Show Tickets' (ID: 456) available. Would you like more details on one of these?

---

**👤 You:**
> "Get the details for booking ID 'BK-55221'."

**🤖 AI Agent:**
> Fetching booking BK-55221... It is a confirmed booking for 'City Tour' scheduled for 2024-12-10, assigned to customer 'Robert Smith'.

---

**👤 You:**
> "Create a booking for product 789 on 2025-01-15 for Alice Brown (alice@email.com)."

**🤖 AI Agent:**
> I've successfully created the booking for Alice Brown. The booking ID is BK-99887. The tickets have been reserved for the requested date.


## ❓ FAQ

**Q: Can I retrieve full metadata for a specific product?**
Yes, use the `get_product` tool with the product ID to get all technical and commercial details associated with that item.

**Q: Is it possible to automate new bookings through the AI?**
Absolutely. The `create_booking` tool allows you to specify the product, date, ticket types, and customer information to generate a booking instantly.

**Q: How can I access customer information?**
You can use `list_customers` to browse your customer database or `get_customer` with a specific ID to see a detailed profile and history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smeetz](https://vinkius.com/mcp/smeetz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smeetz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smeetz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smeetz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smeetz": {
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

# Restful Booker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/restful-booker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage hotel bookings via the Restful Booker API—create, retrieve, update, and delete reservations directly from your AI agent.

## Description
Connect to the **Restful Booker** API to manage hotel reservations. This server allows your AI agent to handle the full lifecycle of bookings, from initial creation to final deletion.

### What you can do

- **Booking Discovery** — List all booking IDs or filter by guest names and dates using `get_booking_ids`
- **Detailed Inspection** — Retrieve full metadata, pricing, and dates for any specific reservation with `get_booking`
- **Reservation Creation** — Instantly create new entries in the system using `create_booking`
- **Flexible Updates** — Modify existing bookings entirely with `update_booking` or change specific fields with `partial_update_booking`
- **Secure Access** — Generate authentication tokens via `create_token` to authorize sensitive write and delete operations

### How it works

1. Subscribe to this server
2. Use the `create_token` tool with your credentials to get an access token
3. Start managing hotel data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — testing API integrations and CRUD workflows in a reliable sandbox environment
- **QA Engineers** — automating reservation scenarios and data validation through natural language
- **Hospitality Tech Teams** — prototyping AI-driven booking assistants and management tools


## Available Tools (8)
- **get_booking**: Get a specific booking
- **health_check**: API health check
- **partial_update_booking**: Requires auth token.

Partially update a booking
- **create_booking**: Create a new booking
- **create_token**: Create a new auth token
- **delete_booking**: Requires auth token.

Delete a booking
- **get_booking_ids**: Can take optional query strings to search.

Get all booking IDs
- **update_booking**: Requires auth token.

Update a current booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restful Booker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all booking IDs for guests with the last name 'Smith'."

**🤖 AI Agent:**
> I found 3 booking IDs for 'Smith': 45, 102, and 215. Would you like me to fetch the full details for any of these?

---

**👤 You:**
> "Create a new booking for John Doe, price 150, deposit paid, from 2024-12-01 to 2024-12-05."

**🤖 AI Agent:**
> Booking successfully created! The new booking ID is 882. The guest is John Doe with a check-in on Dec 1st and check-out on Dec 5th.

---

**👤 You:**
> "Update booking 882 to change the total price to 200."

**🤖 AI Agent:**
> I've updated the total price for booking 882 to 200 using a partial update. All other details remain the same.


## ❓ FAQ

**Q: How do I find a booking ID for a specific guest?**
Use the `get_booking_ids` tool. You can provide optional parameters like `firstname` or `lastname` to filter the results and find the exact ID you need.

**Q: Do I need an auth token to view booking details?**
No, `get_booking` and `get_booking_ids` are public queries. You only need a token generated via `create_token` for `update_booking`, `partial_update_booking`, and `delete_booking` actions.

**Q: Can I update only the price of a booking without changing other details?**
Yes! Use the `partial_update_booking` tool. It allows you to send only the fields you want to change, such as `totalprice`, while keeping the rest of the booking intact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/restful-booker](https://vinkius.com/mcp/restful-booker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restful Booker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restful-booker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restful Booker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restful-booker": {
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

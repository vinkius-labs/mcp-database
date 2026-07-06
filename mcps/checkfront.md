# Checkfront MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkfront)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage tour bookings, activity availability, rental items, customers, and categories for your Checkfront platform through natural conversation.

## Description
Connect your **Checkfront** booking platform to any AI agent — for tours, activities, and rentals.

### What you can do
- **Bookings** — Browse reservations with customer, date, group size, and payment
- **Items** — List all bookable experiences, tours, and rentals
- **Availability** — Check open slots for any experience and date range
- **Categories** — Tours, activities, rentals, classes, events
- **Customers** — Search profiles with booking history
- **Account** — Business configuration and settings


## Available Tools (8)
- **list_bookings**: "What tours are booked for Saturday?"

List bookings
- **get_booking**: Get booking details
- **list_items**: "What do we offer?"

List bookable items
- **get_item**: Get item details
- **get_account**: Get account info
- **check_availability**: Check availability
- **list_categories**: With item counts.

List categories
- **search_customers**: Returns contact, booking history, total spend, and waivers on file.

Search customers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkfront** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What tours are booked for this Saturday and how many spots are left?"

**🤖 AI Agent:**
> 🎯 **Saturday Bookings — Oct 19**

1. 🌊 **Whale Watching Tour** — 9:00 AM
   👥 18/24 booked | 6 spots left | $95/person

2. 🍷 **Wine Country Tour** — 10:30 AM
   👥 12/12 booked | **SOLD OUT** | $125/person

3. 🚴 **Mountain Bike Adventure** — 2:00 PM
   👥 4/8 booked | 4 spots left | $75/person

---

**👤 You:**
> "List all customers who booked the Sunset Cruise next week."

**🤖 AI Agent:**
> Found 12 upcoming bookings for Sunset Cruise next week. The manifest includes: John Adams (4 tix), Maria Silva (2 tix), the O'Connor family (6 tix). Total revenue: $840 collected.

---

**👤 You:**
> "Are there any kayak rentals left for August 15th afternoon?"

**🤖 AI Agent:**
> Checking inventory for August 15th (12:00 PM - 5:00 PM)... Yes, there are exactly 9 double kayaks and 4 single kayaks available for booking.


## ❓ FAQ

**Q: What businesses use Checkfront?**
Checkfront is used by tour operators, activity providers, rental companies, and experience businesses worldwide to manage online booking and inventory.

**Q: Can I query available slots for a given rental gear category?**
Yes! The MCP directly interfaces with the Checkfront Item/Category API. You can ask exactly how many mountain bikes or kayaks remain available for next Saturday.

**Q: Will an AI cancellation automatically refund my guest's payment?**
By default, the AI cancels the booking status but defers payment refunds to your manual Payment Gateway configuration out of safety, unless strictly instructed other configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkfront](https://vinkius.com/mcp/checkfront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Checkfront** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `checkfront` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Checkfront** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "checkfront": {
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

# FareHarbor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fareharbor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage tour and activity bookings via FareHarbor — list companies, query availability, and handle bookings directly from your AI agent.

## Description
Connect your **FareHarbor** affiliate or partner account to any AI agent and take full control of your tour and activity bookings through natural conversation.

### What you can do

- **Operator Discovery** — List all authorized tour companies and operators in your network
- **Live Inventory Access** — Query specific tours (items) and check real-time availability for any date or range
- **Seamless Booking** — Create new bookings with customer details and ticket types directly from the cloud
- **Availability Inspection** — Fetch granular details for specific time slots including pricing and remaining capacity
- **Booking Management** — List recent bookings and retrieve detailed status by UUID flawlessy
- **User Context** — Verify your API application and user identity credentials through the agent

### How it works

1. Subscribe to this server
2. Enter your FareHarbor App Key and User Key (received from support@fareharbor.com)
3. Start managing your activity bookings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Affiliates** — quickly find and book activities for clients without leaving your communication tools
- **OTA Developers** — integrate live booking data directly into your AI-powered concierge workflow
- **Operations Teams** — monitor booking statuses and operator availability through simple natural language queries


## Available Tools (11)
- **create_booking**: Create a new booking for a tour or activity
- **get_availability**: Get details for a specific availability slot
- **get_booking**: Get details for a specific booking by UUID
- **get_item_details**: Get details for a specific tour or activity
- **get_me**: Get current API user/affiliate identity
- **list_availabilities_by_date**: List available slots for an item on a specific date
- **list_availabilities_by_range**: List available slots for an item within a date range
- **list_bookings**: List recent bookings for a company
- **list_companies**: List all companies (operators) authorized for booking
- **list_items**: List all tours or activities (items) for a specific company
- **list_lodgings**: List lodging/pickup locations for a company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FareHarbor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the tour companies I can book for."

**🤖 AI Agent:**
> I've retrieved your authorized operators. You can book for 'Island Adventures' (shortname: island-adv) and 'Mountain Treks' (shortname: mountain-treks). Which company's items would you like to see?

---

**👤 You:**
> "Check availability for the Whale Watching tour tomorrow."

**🤖 AI Agent:**
> Searching availability for tomorrow... I found two slots: 9:00 AM (15 spots left) and 2:00 PM (8 spots left). Would you like to proceed with a booking for any of these?

---

**👤 You:**
> "Show me the details for booking UUID abc-123."

**🤖 AI Agent:**
> Retrieving booking... UUID abc-123 is a confirmed reservation for 'John Doe' on the Sunset Cruise. Status is PAID and the customer has been sent their confirmation email.


## ❓ FAQ

**Q: How do I request FareHarbor API access?**
API access is not public. You must email support@fareharbor.com with your business use case to receive your unique App Key and User Key.

**Q: Is there a sandbox environment for testing?**
Yes, FareHarbor provides a demo environment at demo.fareharbor.com. You can use this host with your sandbox credentials to test bookings safely.

**Q: What is a 'shortname' in FareHarbor?**
A shortname is a unique identifier for a specific tour operator or company on the FareHarbor platform. You can find it in the company metadata or dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fareharbor](https://vinkius.com/mcp/fareharbor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FareHarbor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fareharbor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FareHarbor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fareharbor": {
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

# Tock Reservations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tock-reservations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage restaurant reservations, track guest profiles, and monitor business metrics via the Tock API.

## Description
Integrate **Tock**, the leading reservation and hospitality management platform, directly into your AI workflow. Manage your restaurant or venue reservations and guest directory, track special events and pop-ups, monitor real-time business metrics and occupancy rates, and oversee your hospitality operation using natural language.

### What you can do

- **Reservation Oversight** — List and retrieve detailed information, party sizes, and statuses for all your business reservations.
- **Guest Intelligence** — Monitor guest profiles and history, resolving names, contact details, and total visit counts across your venues.
- **Performance Management** — Access real-time business metrics, resolving total covers, average check size, and occupancy telemetry via chat.
- **Hospitality Auditing** — Retrieve high-level summaries of reservation volume, event activity, and organizational hospitality health instantly.

### How it works

1. Connect the Tock integration to your AI assistant.
2. Authorize using your Tock REST API Key (found in your business dashboard settings).
3. Orchestrate your guest experience and reservation strategy through intuitive conversation.

### Who is this for?

- **Restaurant Managers** — Quickly check daily covers and upcoming reservation counts on the go.
- **Maître d's & Hosts** — Research guest notes and visit history via chat to personalize service.
- **Operations Teams** — Monitor occupancy trends and organizational hospitality metadata instantly.


## Available Tools (10)
- **get_tock_account_metadata**: Retrieve metadata and limits for your Tock account
- **get_business_performance_metrics**: Get a summary of performance metrics for a specific business
- **get_business_detailed_data**: Get detailed settings and information for a specific business
- **quick_hospitality_volume_audit**: Retrieve a high-level summary of reservations, guests, and events
- **get_reservation_details**: Get full content and status for a specific reservation
- **list_managed_businesses**: List all businesses and venues managed in your Tock account
- **list_business_special_events**: List all special events and pop-ups for a specific business
- **list_business_guests**: List all guests registered in the business directory
- **list_business_reservations**: List all reservations for a specific business
- **list_future_scheduled_reservations**: Identify reservations that are scheduled for a future date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tock Reservations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reservations for tonight."

**🤖 AI Agent:**
> I've found 15 reservations for tonight, including a party of 4 for 'John Miller' (7:00 PM) and a party of 2 for 'Alice Connor' (8:30 PM). Total expected covers: 45. Would you like to see the guest notes for John Miller?

---

**👤 You:**
> "What are our performance metrics for this week?"

**🤖 AI Agent:**
> This week across your business, you have 350 total covers with an occupancy rate of 85%. The average check size is $75. Performance is up 10% compared to last week. Should I pull the breakdown by day of the week?

---

**👤 You:**
> "Search for guest 'Sarah Connor'."

**🤖 AI Agent:**
> Sarah Connor has visited your venues 5 times. Their last visit was on March 15th at the 'Downtown Bistro'. They are flagged as a 'VIP Guest'. Would you like to see their dietary preferences and special notes?


## ❓ FAQ

**Q: How do I get a Tock API Key?**
Log in to your Tock dashboard as an administrator, navigate to **Settings > API**, and you can generate or retrieve your unique **REST API Key** from there. Ensure you have an active business subscription.

**Q: Does the integration show guest dietary preferences?**
Yes, you can use the get_reservation_details tool to retrieve specific guest notes, which typically include dietary restrictions, special occasions, and seating preferences.

**Q: Can the agent make new reservations?**
This integration currently focuses on listing and auditing existing reservations, guests, and events. Making new reservations or processing payments should be handled via the Tock booking widget or dashboard interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tock-reservations](https://vinkius.com/mcp/tock-reservations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tock Reservations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tock-reservations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tock Reservations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tock-reservations": {
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

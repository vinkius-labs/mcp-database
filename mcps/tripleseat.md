# Tripleseat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tripleseat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Manage event bookings, leads, contacts, venues, and accounts for your Tripleseat event management platform through natural conversation.

## Description
Connect your **Tripleseat** account to any AI agent — the leading event management platform.

### What you can do
- **Events** — Browse upcoming events with menus, AV, and BEOs
- **Bookings** — Room assignments, setup styles, and time blocks
- **Leads** — Sales pipeline with event type, budget, and response status
- **Contacts** — Event planner CRM with history and revenue
- **Venues** — Multi-location management with rooms and capacity
- **Accounts** — Corporate client tracking with total spend


## Available Tools (8)
- **list_events**: "What events this week?"

List events
- **get_event**: Get event details
- **list_bookings**: For venue calendar.

List bookings
- **get_booking**: Get booking details
- **list_leads**: For sales pipeline.

List event leads
- **search_contacts**: CRM for event planners.

Search contacts
- **list_locations**: For multi-venue management.

List event venues
- **list_accounts**: List accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tripleseat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What events do we have this week?"

**🤖 AI Agent:**
> 🎪 **This Week's Events**

1. 💍 **Johnson Wedding** — Sat Oct 19, Grand Ballroom
   👥 150 guests | 💰 $12,500 | 🍽️ Plated dinner + bar

2. 🏢 **Acme Corp Q3 Review** — Thu Oct 17, Private Room
   👥 35 guests | 💰 $2,800 | 🍽️ Buffet lunch

3. 🎂 **Elena's 40th Birthday** — Fri Oct 18, Patio
   👥 60 guests | 💰 $4,200 | 🍽️ Cocktail reception

---

**👤 You:**
> "List all confirmed private events in the Main Dining Room for next week."

**🤖 AI Agent:**
> Querying Tripleseat reservations ('get_events')...
Found 2 confirmed private events for the 'Main Dining Room' next week:
1. 'Smith Wedding Rehearsal' - Thursday, 6 PM - 50 guests.
2. 'Acme Corp Corporate Dinner' - Saturday, 7 PM - 120 guests.

---

**👤 You:**
> "Create a new lead for a 30-person birthday party on October 12th under 'Jane Doe'."

**🤖 AI Agent:**
> Executing `create_lead` operational constraint...
Lead successfully recorded in Tripleseat.
Type: Birthday Party
Date: Oct 12th
Guest count: 30
Contact Name: Jane Doe
Assigned Lead ID: `lead-7719`.


## ❓ FAQ

**Q: What is Tripleseat?**
Tripleseat is the leading cloud event management and catering platform for restaurants and hotels. Used by thousands of venues for private dining, weddings, corporate events, and banquets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tripleseat](https://vinkius.com/mcp/tripleseat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tripleseat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tripleseat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tripleseat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tripleseat": {
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

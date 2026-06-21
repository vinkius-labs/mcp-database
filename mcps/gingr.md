# Gingr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gingr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Retrieve pet owner profiles, track reservations, and oversee check-ins via AI agents with Gingr.

## Description
Connect your **Gingr** pet care management account to any AI agent to automate your data extraction and customer support workflows through the Model Context Protocol (MCP). Gingr is the leading platform for kennel, daycare, and grooming businesses. This MCP server enables you to retrieve detailed pet owner profiles, track upcoming and past reservations, and monitor real-time facility check-ins directly through natural conversation.

### Key Features

- **Owner & Pet Insights** — Retrieve complete profile metadata for pet owners using IDs, email addresses, or phone numbers.
- **Reservation Tracking** — List all boarding, daycare, and grooming reservations for any owner, filtered by status (future or currently checked-in).
- **Digital Whiteboard Oversight** — Access 'Back of House' data to see real-time facility activity and room assignments for any location.
- **Custom Data Discovery** — Search across custom metadata fields for both owners and animals to find specific regional or internal attributes.
- **Facility Transparency** — List all business locations and facilities configured in your Gingr app.
- **Read-only Security** — Safely query your pet care database with a secure, read-only integration designed for data visibility.
- **Real-time Synchronization** — Keep your facility operations data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gingr Subdomain and API Key (found in User Settings)
3. Start querying your pet care data from Claude, Cursor, or any MCP client

### Who is this for?

- **Pet Care Facility Managers** — quickly check check-in statuses or room assignments without manual dashboard navigation.
- **Customer Support Teams** — get a real-time overview of an owner's reservation history via simple AI commands.
- **Operations Leads** — automate the retrieval of facility activity data for daily reporting.


## Available Tools
- **verify_api_connection**: Check connection
- **list_active_checkins**: List currently checked-in
- **find_owner_by_email**: Search owner by email
- **get_pet_owner_details**: Get owner profile
- **find_owner_by_phone**: Search owner by phone
- **get_digital_whiteboard**: View active whiteboard
- **list_business_locations**: List pet care facilities
- **list_owner_reservations**: ) for a specific owner.

List past/future bookings
- **search_pet_custom_fields**: Search custom pet data
- **search_owner_custom_fields**: Search custom owner data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gingr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find pet owner details for 'john@email.com'."

**🤖 AI Agent:**
> Retrieving owner... I found a profile for John Doe. He has one pet named 'Buddy' (Golden Retriever) and his last check-in was yesterday.

---

**👤 You:**
> "List all future reservations for owner ID '12345'."

**🤖 AI Agent:**
> Fetching reservations... Owner 12345 has 2 upcoming bookings: a 3-day boarding stay starting next Friday and a grooming session on Monday.

---

**👤 You:**
> "Show me the current digital whiteboard for location '1'."

**🤖 AI Agent:**
> Retrieving whiteboard... In location 1, there are currently 12 pets checked-in for daycare and 5 for boarding. 3 pets are currently assigned to the 'Blue Room'.


## ❓ FAQ

**Q: How do I get an API Key for Gingr?**
Log in to Gingr, navigate to Reports & More > Users, edit your user, and look for the 'API Keys' section to generate or copy your key.

**Q: Can I create new reservations via the agent?**
No, the current Gingr Public API is read-only. This integration is designed for safely retrieving and auditing your existing data.

**Q: How do I find my Location ID?**
Use the 'list_business_locations' tool. The agent will return all configured locations in your app along with their unique IDs.

**Q: Is the Digital Whiteboard data live?**
Yes, all data retrieved through the 'get_digital_whiteboard' tool is fetched directly from the Gingr API, reflecting the current state of your facility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gingr](https://vinkius.com/mcp/gingr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gingr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gingr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gingr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gingr": {
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

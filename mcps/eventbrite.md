# Eventbrite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventbrite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage events, track attendees, and monitor ticket orders via the Eventbrite API.

## Description
Integrate **Eventbrite**, the world's leading event management and ticketing platform, directly into your AI workflow. Manage your live and upcoming events, track registered attendees and ticket orders, monitor performance metrics and gross sales, and oversee your organizational event calendar using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, venues, and status for all your Eventbrite events.
- **Attendee Intelligence** — Monitor registered attendees, resolving names, emails, and ticket types across your events.
- **Order Management** — Access and monitor ticket orders and transactions, tracking real-time sales and payment statuses.
- **Event Auditing** — Retrieve high-level summaries of event volume, attendance trends, and organizational account health instantly.

### How it works

1. Connect the Eventbrite integration to your AI assistant.
2. Authorize using your Eventbrite Private Token (found in your account settings).
3. Orchestrate your event strategy and ticketing operations through intuitive conversation.

### Who is this for?

- **Event Organizers** — Quickly check attendee counts and event statuses on the go.
- **Marketing Teams** — Research event performance and sales telemetry via chat during campaign optimization.
- **Operations Teams** — Monitor ticket orders and organizational event metadata instantly.


## Available Tools
- **get_eventbrite_account_metadata**: Retrieve metadata and profile information for the current Eventbrite user
- **get_event_performance_summary**: Get a summary of performance metrics for a specific event
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **list_my_organizations**: List all organizations the user is a member of on Eventbrite
- **quick_event_volume_audit**: Retrieve a high-level summary of upcoming events and attendance
- **list_event_attendees**: List all registered attendees for a specific event
- **list_currently_live_events**: Identify events that are currently in a "Live" or "Started" status
- **list_event_ticket_orders**: List all ticket orders and transactions for a specific event
- **list_past_completed_events**: Identify events that have already taken place
- **list_my_events**: List all events created or managed by the authenticated user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventbrite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming live events."

**🤖 AI Agent:**
> I've found 3 live events, including 'Annual Tech Summit' and 'Digital Marketing Workshop'. The Tech Summit has 450 registered attendees. Would you like to see the ticket sales summary for the workshop?

---

**👤 You:**
> "Show me the attendee list for event ID '12345678'."

**🤖 AI Agent:**
> For event ID '12345678', I've retrieved the list of 120 attendees, including 'John Doe', 'Jane Smith', and 'Robert Brown'. All attendees have 'Completed' status. Should I pull the ticket type breakdown?

---

**👤 You:**
> "Check the performance summary for 'Summer Gala'."

**🤖 AI Agent:**
> The 'Summer Gala' has sold 850/1000 tickets, generating $42,500 in gross sales. 15 orders were placed in the last 24 hours. Would you like a list of the most recent orders?


## ❓ FAQ

**Q: How do I get an Eventbrite Private Token?**
Log in to your Eventbrite account, navigate to **Account Settings > API Keys**, and you can find or generate your **Private Token** (OAuth token) there. Ensure you use the Private Token for authorized access to your data.

**Q: Can the agent create new events?**
This integration currently focuses on listing and auditing events, attendees, and orders. Creating or publishing new events should be managed via the Eventbrite event builder or professional management tools.

**Q: Does the integration show real-time gross sales?**
Yes, you can use the get_event_performance_summary tool to retrieve a summary of gross sales, total tickets sold, and other revenue metrics for a specific event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventbrite](https://vinkius.com/mcp/eventbrite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eventbrite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eventbrite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eventbrite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventbrite": {
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

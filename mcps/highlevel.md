# HighLevel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highlevel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Automate CRM and marketing via HighLevel — manage contacts, opportunities, and calendars directly from any AI agent.

## Description
Connect your **HighLevel** (GoHighLevel) account to any AI agent and take full control of your sales pipeline, contact management, and scheduling through natural conversation.

### What you can do

- **Contact Oversight** — Perform advanced searches for leads, retrieve full profiles, and create new contact records effortlessly.
- **Sales Pipelines** — List pipelines and search for opportunities to monitor your deals and revenue flow.
- **Appointment Management** — Access your calendars, check for free slots in real-time, and book appointments directly from the chat.
- **Task Coordination** — List and create tasks for specific contacts to ensure follow-ups are never missed.
- **Location Tracking** — Retrieve location-specific tags to categorize and filter your data accurately.
- **Unified CRM** — Bridge the gap between your marketing and sales activities using the powerful API v2.

### How it works

1. Subscribe to this server
2. Enter your HighLevel API v2 Access Token
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

No more jumping between complex dashboard views. Your AI assistant acts as a dedicated Sales Assistant or Marketing Operations Lead.

### Who is this for?

- **Marketing Agencies** — instantly retrieve lead details and opportunity statuses for multiple clients.
- **Sales Reps** — automate the process of logging follow-up tasks and booking meetings.
- **Business Owners** — maintain a real-time overview of their sales funnel and appointments.


## Available Tools (11)
- **create_appointment**: Book a new appointment on a calendar
- **create_contact**: Pass payload as JSON string in "body_json" (requires firstName, email, or phone).

Add a new contact/lead to HighLevel
- **create_contact_task**: Assign a new task to a specific contact
- **get_contact_details**: Get detailed information for a specific contact
- **get_calendar_free_slots**: Check availability for a specific calendar
- **list_calendars**: List all calendars available for a location
- **list_contact_tasks**: List all tasks assigned to a specific contact
- **list_pipelines**: List sales pipelines for a specific location
- **list_location_tags**: List all custom tags for a location
- **search_contacts**: Pass search criteria as a JSON string in "search_json".

Search for contacts in HighLevel
- **search_opportunities**: Search for opportunities within a pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HighLevel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for contact 'John Doe' and show his pending tasks."

**🤖 AI Agent:**
> I've found John Doe (ID: contact_123). He currently has 2 pending tasks: 'Follow-up on quote' (Due tomorrow) and 'Send welcome kit'. Would you like to create a new task for him?

---

**👤 You:**
> "Find free slots on the 'Sales Consultation' calendar for next Monday."

**🤖 AI Agent:**
> Checking availability... For next Monday (April 12th), I found 3 free slots: 10:00 AM, 02:30 PM, and 04:00 PM. Should I book an appointment for a specific contact?

---

**👤 You:**
> "Show me all opportunities in the 'Product Sales' pipeline."

**🤖 AI Agent:**
> Accessing pipeline... I found 5 active opportunities in 'Product Sales', totaling $12,500 in potential value. 2 deals are in 'Discovery' and 3 are in 'Proposal Sent'. Would you like to see the details for the largest deal?


## ❓ FAQ

**Q: How do I find my HighLevel API v2 Access Token?**
You can obtain an API v2 Access Token by creating an application in the **HighLevel Developer Portal** (marketplace.gohighlevel.com) and performing the OAuth 2.0 handshake. Ensure you grant the necessary scopes for contacts and opportunities.

**Q: Can I check calendar availability in real-time?**
Yes! Use the `get_calendar_free_slots` tool by providing the calendar ID and a date range. The agent will return all available appointment slots for that period.

**Q: Does the integration support creating new opportunities?**
Yes, you can use the `create_opportunity` tool. You must provide a JSON string containing the pipeline ID, stage ID, and contact details to add a new deal to your sales funnel.

**Q: Is the integration secure for CRM data?**
Absolutely. The integration uses official HighLevel API v2 OAuth 2.0 Bearer tokens over HTTPS. Your credentials and customer data are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highlevel](https://vinkius.com/mcp/highlevel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HighLevel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `highlevel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HighLevel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "highlevel": {
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

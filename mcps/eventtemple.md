# EventTemple MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventtemple)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Fill your venue calendar with event bookings, catering orders, and banquet management tools made for hospitality sales teams.

## Description
Connect your **EventTemple** account to any AI agent and take full control of your hospitality sales and catering management workflows through natural conversation.

### What you can do

- **Booking Orchestration** — List and manage group bookings programmatically, including retrieving detailed metadata about statuses, dates, and account associations
- **Event Intelligence** — Access individual catering events and schedules to coordinate venue requirements and maintain a high-fidelity operational flow
- **Relationship CRM** — Manage complete profiles for contacts and accounts to maintain high-touch relationships and track communication history
- **Task & Activity Tracking** — Retrieve and manage associated tasks and internal notes to ensure every detail of the event planning process is captured
- **Financial Visibility** — Monitor the financial health of your bookings by listing and inspecting associated invoices directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your EventTemple settings (Settings > Integrations or Developer)
3. Start managing your hospitality business from Claude, Cursor, or any MCP client

No more manual deal logging or digging through complex catering tables. Your AI acts as your dedicated sales and catering coordinator.

### Who is this for?

- **Hotel Sales Teams** — instantly retrieve group lead details and update booking statuses using natural language commands
- **Event Planners** — quickly access event schedules and venue requirements without leaving your communication tools
- **Venue Managers** — monitor upcoming event pipelines and track financial tasks through simple AI queries


## Available Tools
- **get_booking**: Get booking details
- **get_contact**: Get contact details
- **get_event**: Get event details
- **list_accounts**: List all accounts/companies
- **list_bookings**: List all bookings
- **list_contacts**: List all contacts
- **list_events**: List all individual events
- **list_invoices**: List all invoices
- **list_tasks**: List all tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EventTemple** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my group bookings in EventTemple."

**🤖 AI Agent:**
> I've retrieved your bookings. You currently have 4 active groups, including 'Tech Global Summit' (Tentative) and 'Marketing Awards 2026' (Confirmed). Which one should I check the events for?

---

**👤 You:**
> "Show me the details for booking ID 'bk_123'."

**🤖 AI Agent:**
> Fetching booking bk_123... This group is for the 'Smith Wedding' with a total of 120 guests. It includes a ceremony in the Courtyard and a dinner in the Grand Hall. Would you like to see the associated tasks?

---

**👤 You:**
> "List all individual events for next month."

**🤖 AI Agent:**
> Scanning your calendar... For next month, I found 5 scheduled events, including 2 Gala Dinners and 3 Corporate Meetings. Shall I provide the venue and setup details for these?


## ❓ FAQ

**Q: How do I find my EventTemple API Key?**
Log in to your account, navigate to **Settings** > **Integrations** or the **Developer** section, and click **Generate API Key**.

**Q: Does the integration support viewing event tasks?**
Yes! Use the `list_tasks` tool to retrieve all pending and completed activities associated with your bookings programmatically.

**Q: Can I list individual contacts for an account?**
The `list_contacts` tool retrieves your directory of clients. You can ask your agent to filter or find specific records associated with an account ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventtemple](https://vinkius.com/mcp/eventtemple)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EventTemple** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eventtemple` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EventTemple** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventtemple": {
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

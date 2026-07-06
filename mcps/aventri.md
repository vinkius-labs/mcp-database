# Aventri MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aventri)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage events, contacts, and speakers via Aventri — list events, search contacts, and clone event modules directly from your AI agent.

## Description
Connect your **Aventri** (now Stova) account to any AI agent to streamline your event management and attendee coordination through natural language.

### What you can do

- **Event Management** — List all events, search for specific ones by name or date, and clone existing events including specific modules for rapid setup.
- **Contact & Attendee CRM** — Add, update, or delete contacts. Retrieve detailed profiles and search your database by email or unique identifiers.
- **Speaker Coordination** — List all account-level speakers, fetch detailed session associations, and create new speaker profiles instantly.
- **Pre-Approval Workflows** — Manage pre-load and pre-approved lists to ensure smooth registration and access control.

### How it works

1. Subscribe to this server
2. Enter your Aventri Account ID and API Key
3. Start orchestrating your conferences and meetings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — quickly duplicate successful event structures and manage speaker lists without manual data entry.
- **Marketing Operations** — sync contact data and manage attendee lists directly from your workflow tools.
- **Executive Assistants** — retrieve event details and speaker bios for briefings using simple conversational queries.


## Available Tools (13)
- **clone_event**: Clone an existing event
- **create_speaker**: Create an account-level speaker
- **delete_contact**: Delete a contact from the system
- **get_contact**: Get detailed information for a specific contact
- **get_speaker**: Get speaker details and associated sessions
- **list_contacts**: List contacts in the Aventri account
- **list_events**: List all events in the account
- **list_speakers**: List all speakers associated with the account
- **search_events**: Search and filter events
- **update_contact**: Update an existing contact
- **add_contact**: Add a new contact to the account or database
- **add_pre_approved**: Add contacts to a pre-approved list
- **add_pre_load**: Add pre-load registrant data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aventri** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all events currently in my Aventri account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 active events: 'Global Tech Summit 2024' (ID: 8821), 'Annual Partner Meetup' (ID: 9932), and 'Developer Workshop' (ID: 10443).

---

**👤 You:**
> "Find the contact details for the user with email 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching contacts... I found John Doe (Contact ID: 55402). He is registered as a 'Senior Manager' at 'Example Corp'. Would you like to see his full profile?

---

**👤 You:**
> "Clone event 8821 and call it 'Global Tech Summit 2025'."

**🤖 AI Agent:**
> I am initiating the clone process for event 8821. I will duplicate the core modules to create your new 2025 event instance. One moment...


## ❓ FAQ

**Q: Can I search for specific events by name or date range?**
Yes! Use the `search_events` tool. You can filter by name, event ID, folder, or specific dates to find exactly what you need.

**Q: How do I duplicate an existing event structure?**
You can use the `clone_event` tool. Simply provide the `eventid` of the source event and optionally specify which modules you want to include in the copy.

**Q: Is it possible to manage speaker profiles and their sessions?**
Absolutely. You can use `list_speakers` to see everyone, `get_speaker` to see specific session assignments, and `create_speaker` to add new talent to your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aventri](https://vinkius.com/mcp/aventri)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aventri** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aventri` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aventri** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aventri": {
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

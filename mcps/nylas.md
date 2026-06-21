# Nylas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nylas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Equip your AI agent to manage emails, calendars, and contacts across all providers (Gmail, Outlook) through a single unified interaction.

## Description
Connect your **Nylas** account to your AI agent and seamlessly interact with communication data across 100% of email and calendar providers.

### What you can do

- **Email Management** — Use `list_messages` to read inbound emails, navigate through `list_folders` and `list_drafts`, or actively compose and dispatch emails live using `send_message`.
- **Calendar Syncing** — Fetch meeting tracking arrays via `list_calendars` and `list_events`, or actively block out new times by invoking `create_event`.
- **Contact Organization** — Rapidly enumerate directory users with `list_contacts` and insert newly met stakeholders via `create_contact` natively.

### How it works

1. Subscribe to this server
2. Enter your Nylas API Key (v3)
3. Start managing your cross-provider email and calendar architecture using Claude, Cursor, or your preferred AI client

### Who is this for?

- **Sales Development Reps** — automate email drafting, verify outbound calendar slots, and log contact information in seconds.
- **Founders & Executives** — triage the morning inbox securely, block out focus time on the calendar, and schedule meetings conversationally.
- **HR & Recruiting** — track candidate communications effectively and seamlessly schedule multi-party interviews directly from the terminal.


## Available Tools
- **list_calendars**: Returns internal calendar UUIDs required to execute event queries.

List all user calendars connected via Nylas
- **list_events**: List scheduled events mapped inside a specific Calendar UUID
- **create_event**: g. Google Calendar).

Create a new synchronized calendar event
- **delete_event**: Delete a specific calendar event from the provider
- **list_messages**: Retrieve the unified inbox/messages stream for the authenticated grant
- **send_message**: Dispatch an outbound email utilizing the native mail provider
- **list_contacts**: List natively synced address book contacts from the user account
- **create_contact**: Insert a brand new address book contact record
- **list_folders**: Enumerate the organizational email directories tracking labels/files
- **list_drafts**: Dump unsent email threads parked in the Drafts bound location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nylas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my inbox for any emails received today with the subject 'Invoice'."

**🤖 AI Agent:**
> I've fetched your latest messages and found 2 emails containing 'Invoice' received today. Would you like me to summarize the billing amounts?

---

**👤 You:**
> "Schedule a 30-minute sync at 2 PM tomorrow titled 'Q3 Execution Strategy'."

**🤖 AI Agent:**
> Your calendar event 'Q3 Execution Strategy' is now scheduled for tomorrow at 2:00 PM successfully.

---

**👤 You:**
> "Find Robert's email address by listing my contacts."

**🤖 AI Agent:**
> I checked your Nylas contact directory. Robert's formal email address is `robert.smith@domain.com`. Would you like me to draft a message to him?


## ❓ FAQ

**Q: Can my AI draft and actually send emails natively?**
Yes! Provide the recipient, subject, and prompt your agent on what the body should look like. The agent leverages the `send_message` tool interacting directly through the Nylas provider, and your real account will dispatch the email in seconds.

**Q: How can I check if I have upcoming meeting clashes?**
Your agent queries your complete agenda using the `list_events` tool. Describe your timeframe, and the AI will scan down the returned events, identifying overlapping blocks or showing you pure free space availability.

**Q: Will the agent read my historical email archives?**
When using `list_messages`, the agent fetches paginated incoming boxes. You can search directly by providing queries within the prompt, letting the agent fetch and summarize the content of past conversation threads effectively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nylas](https://vinkius.com/mcp/nylas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nylas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nylas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nylas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nylas": {
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

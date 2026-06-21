# Eventee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage events, track speakers, and monitor attendee engagement via the Eventee API.

## Description
Integrate **Eventee**, the leading mobile-first event management platform, directly into your AI workflow. Manage your event schedules and sessions, track registered speakers and attendees, monitor audience questions and partner sponsorships, and oversee your event engagement using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, dates, and status for all your Eventee projects.
- **Speaker & Session Intelligence** — Monitor event schedules, resolving session titles, speaker bios, and unique identifiers.
- **Engagement Management** — Access and monitor audience questions and attendee registration progress in real-time.
- **Event Auditing** — Retrieve high-level summaries of session volume, speaker diversity, and organizational event health instantly.

### How it works

1. Connect the Eventee integration to your AI assistant.
2. Authorize using your Eventee API Key (found in your account settings).
3. Orchestrate your event planning and mobile engagement strategy through intuitive conversation.

### Who is this for?

- **Event Planners** — Quickly check session schedules and speaker details on the go.
- **Marketing Teams** — Research attendee engagement and partner visibility via chat during live events.
- **Operations Teams** — Monitor registration counts and organizational event metadata instantly.


## Available Tools (10)
- **get_eventee_account_metadata**: Retrieve metadata and limits for your Eventee account
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_engagement_audit**: Retrieve a high-level summary of sessions, speakers, and attendees
- **list_currently_active_events**: Identify events that are currently taking place
- **list_event_registered_attendees**: List all registered attendees for a specific event
- **list_all_events**: List all events managed in your Eventee account
- **list_event_partners_and_sponsors**: List all partners and sponsors for a specific event
- **list_event_audience_questions**: List all questions submitted by the audience for a specific event
- **list_event_sessions**: List all sessions and schedule items for a specific event
- **list_event_speakers**: List all speakers registered for a specific event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sessions for event ID 'EVENT-12345'."

**🤖 AI Agent:**
> I've found 12 sessions for event 'EVENT-12345', including 'Opening Keynote' (10:00 AM) and 'Product Deep Dive' (2:00 PM). Would you like to see the speakers for the Keynote?

---

**👤 You:**
> "What audience questions have been submitted for today's event?"

**🤖 AI Agent:**
> For today's event, 5 questions have been submitted, including 'How does the new API handle scale?' and 'What is the release date?'. 3 questions are currently awaiting moderation. Should I pull the session IDs they are associated with?

---

**👤 You:**
> "Show me the sponsors for our upcoming conference."

**🤖 AI Agent:**
> I've retrieved 8 partners/sponsors for the upcoming conference, including 'TechCorp' (Platinum), 'InnoVentures' (Gold), and 'Global Solutions'. Would you like the contact information for TechCorp?


## ❓ FAQ

**Q: How do I get an Eventee API Key?**
Log in to your Eventee dashboard, navigate to **Administration > API**, and you can generate or retrieve your unique API Key from there. API access may be restricted to certain plans.

**Q: Can the agent manage live polls?**
This integration currently focuses on listing and auditing events, sessions, and questions. Managing live polls or reacting to real-time interactions should be handled via the Eventee mobile app or administration console.

**Q: Does the integration show attendee details?**
Yes, you can use the list_event_registered_attendees tool to retrieve names and basic registration metadata for all participants of a specific event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventee](https://vinkius.com/mcp/eventee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eventee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eventee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eventee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eventee": {
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

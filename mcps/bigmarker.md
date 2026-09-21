# BigMarker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bigmarker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Run webinar programs from any AI workflow — search and schedule sessions, manage registrations and attendance, and pull reporting from BigMarker.

## Description
Connect your **BigMarker** account to any AI agent so it can run webinar programs end to end — using BigMarker's official API.

### What you can do

- **Discover sessions** — list webinars across channels, search by title or date window, pull full detail for one session
- **Registrations & attendance** — see who registered, who actually attended, and who no-showed
- **Reporting** — per-webinar statistics and the rolled-up event summary (registrations, attendance, chat, Q&A, polls)
- **Channels** — list channels and the webinars inside each one
- **Registration lifecycle** — register an attendee or cancel a registration
- **Scheduling** — create a new webinar in a channel with time zone-aware start times

### How it works

1. Subscribe to this server
2. Generate an **API key** in BigMarker user settings → API Keys
3. Ask your agent: "Who attended last week's product webinar?", "Register ada@lovelace.com for Thursday's session", "What's our no-show rate this month?"

The key is sent in the `API-KEY` header and is scoped to your account.

### Who is this for

- **Marketing & demand-gen teams** — answer webinar performance questions from a chat instead of exporting CSVs
- **Event ops** — register, cancel and check in attendees as part of a larger automation
- **RevOps** — reconcile attendance against your CRM and route engaged attendees to sales


## Available Tools (12)
- **cancel_registration**: This does not delete the attendee record itself — use it to undo a registration made by mistake.

Cancel an attendee’s registration for a webinar
- **create_webinar**: Set start_time as ISO 8601 with the time_zone name (e.g. "America/New_York") so the session lands on the right day locally. The API accepts ~55 optional fields — this tool exposes the ones used most; configure advanced settings in the dashboard afterwards.

Create a new webinar in a channel
- **get_webinar_stats**: For the rolled-up event summary use get_event_summary.

Get attendance and engagement statistics for a webinar
- **get_webinar**: Find the id with list_webinars or search_webinars first.

Get full details for one webinar
- **get_event_summary**: Get the rolled-up reporting summary for a webinar
- **list_attendees**: Paginated with current_page/per_page; set show_chat to include each attendee’s chat messages.

List attendees who joined a webinar
- **list_channel_webinars**: Paginated with page/per_page.

List the webinars in one channel
- **list_channels**: The id from here feeds create_webinar and list_channel_webinars.

List the channels in your BigMarker account
- **list_webinars**: Filter by type, role, or a time window. Use search_webinars instead when you are looking for webinars by title or tag.

List webinars across your BigMarker channels
- **list_registrations**: Filter by email or an updated_since timestamp. For registrations including custom-field answers, see the registrations_with_fields variant in the BigMarker docs.

List registrations for a webinar
- **register_attendee**: Pass custom_fields as a JSON object of the webinar’s registration questions. Use register_or_update in the BigMarker docs for upsert semantics with external ids.

Register an attendee for a webinar
- **search_webinars**: Returns the same paginated conference envelope.

Search webinars by title, tag, presenter, or date window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BigMarker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who actually attended last Thursday's product webinar, and how many registrations were no-shows?"

**🤖 AI Agent:**
> 38 of 52 registrants attended (73% attendance, 14 no-shows). The attendees included 9 people from target accounts — I listed attendees for the session and compared the counts against registrations.

---

**👤 You:**
> "Register ada@lovelace.com for the onboarding webinar on October 1st."

**🤖 AI Agent:**
> Done — ada@lovelace.com is registered for the October 1st onboarding session. I found the webinar by title, then registered her with the name on file.

---

**👤 You:**
> "Spin up a webinar for our October product launch and give me the registration link."

**🤖 AI Agent:**
> Created. The webinar is set up with its title, date and start time on the channel you asked for, and it comes back with its webinar id and the public registration URL — share that link and every signup lands in the registration list, so you can hand out the link now and pull attendance through this same server afterwards.


## ❓ FAQ

**Q: Where do I get my BigMarker API key?**
Sign in to BigMarker, open your user settings and go to **API Keys** to generate a key. Alternatively, POST your account email and password to /api/v1/members/login to receive a token. The key is sent in the API-KEY header.

**Q: What is the difference between list_registrations and list_attendees?**
Registrations are everyone who signed up; attendees are the subset who actually joined the session. Use attendees when you want real presence — for a no-show rate, compare the two counts.

**Q: Can I use this to set up a whole webinar with one prompt?**
You can create the session — create_webinar takes a channel, title, start time, time zone and format. The BigMarker API exposes about 55 optional fields per webinar (webhooks, branding, registration rules); configure those in the dashboard after the session exists.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bigmarker](https://vinkius.com/en/ai-agent-connect/bigmarker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BigMarker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bigmarker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BigMarker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bigmarker": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

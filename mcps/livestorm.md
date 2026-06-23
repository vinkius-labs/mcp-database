# Livestorm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/livestorm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Connect your AI agent to Livestorm to manage webinars, registrations, attendees, and analytics via natural language.

## Description
Integrate **Livestorm**, the leading browser-based webinar and video events platform, directly into your AI workflow. Manage webinar schedules, track registrations, monitor attendee engagement, access real-time analytics, and send replay emails — all through conversational AI.

### What you can do

- **Webinar Management** — List, create, and retrieve all your webinars with scheduling and status information
- **Registration Tracking** — View all registrations for any webinar, create new attendee registrations, and verify individual registration details
- **Attendee Monitoring** — List attendees who actually joined events, track attendance duration and engagement metrics
- **Analytics & Reporting** — Access post-event analytics including registration counts, attendance rates, and replay views
- **Replay Distribution** — Send replay email links to all attendees of completed events with one action
- **Room Management** — List all webinar rooms in your Livestorm workspace for infrastructure planning

### How it works

1. Connect the Livestorm integration to your AI assistant
2. Authorize using your Livestorm API Token (found in Settings → Integrations → API)
3. Manage your webinar ecosystem and track engagement through intuitive conversation

### Who is this for?

- **Marketing Teams** — Monitor registration growth, track attendance rates, and send replay campaigns
- **Event Planners** — Create and manage webinars, verify attendee lists, and audit event health
- **Sales Teams** — Identify engaged attendees and follow up with prospects who attended your product demos
- **Customer Success** — Track training webinar attendance and send replay links to customers who missed sessions


## Available Tools (10)
- **create_event**: Provide at minimum the event title. Optionally specify description, start/end times, and event type (live, replay, or on-demand).

Create a new webinar or event in Livestorm
- **create_registration**: Creates a new registration record for the specified webinar. The registration email must be unique for that webinar.

Register a new attendee for a Livestorm webinar
- **get_event**: Use list_events first to find the correct ID. Returns full event metadata including settings, registration page URL, and status.

Retrieve detailed information for a specific Livestorm webinar or event
- **get_registration**: Returns the full registration record for the specified attendee.

Retrieve details for a specific registration of a Livestorm webinar
- **list_analytics**: Returns registration counts, attendance rates, replay views, and engagement metrics. Useful for post-event reporting and ROI analysis.

Retrieve analytics data for a specific Livestorm webinar
- **list_attendees**: Returns only attendees who joined the event, not just registered attendees. Includes attendance duration and engagement data.

Retrieve the list of attendees who actually attended a Livestorm webinar
- **list_events**: Returns all events (live, replay, scheduled).

Retrieve a list of all webinars and events in your Livestorm account
- **list_registrations**: Returns attendee details including names, emails, and registration status. Useful for verifying attendance lists.

Retrieve all registrations for a specific Livestorm webinar
- **list_webinar_rooms**: Useful for understanding your Livestorm workspace structure.

Retrieve a list of all rooms (webinar rooms) in your Livestorm workspace
- **send_replay**: Sends the replay link to everyone who attended the specified event. Use after live events to share the recording with attendees.

Send a replay email to all attendees of a completed Livestorm webinar


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Livestorm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all upcoming webinars in my Livestorm account."

**🤖 AI Agent:**
> I found 4 upcoming webinars: 'Product Launch Q2' (March 15), 'Customer Onboarding Deep Dive' (March 22), 'Sales Enablement Workshop' (April 5), and 'Engineering AMA' (April 18). Would you like to see the registration count for any of them?

---

**👤 You:**
> "How many people attended last week's webinar?"

**🤖 AI Agent:**
> Last week's 'Product Launch Q2' webinar had 120 registrations with 87 attendees (72.5% attendance rate). Average watch time was 34 minutes. Would you like me to send the replay to all attendees?

---

**👤 You:**
> "Create a new webinar called 'AI Trends 2026' for next month."

**🤖 AI Agent:**
> I've created the webinar 'AI Trends 2026' as a live event. It's now ready in your Livestorm workspace. You can share the registration page and start promoting it. Want me to help you set up a schedule for it?


## ❓ FAQ

**Q: How do I get my Livestorm API Token?**
Log in to [Livestorm](https://app.livestorm.co), go to **Settings** → **Integrations** → **API**, and copy your API Token. API access may require a paid plan.

**Q: What's the difference between registrations and attendees?**
Registrations are people who signed up for the webinar. Attendees are those who actually joined and attended the event. An attendee is always a registrant, but not all registrants become attendees.

**Q: Can I create a new webinar through the AI integration?**
Yes, use the create_event action with at least a title. You can optionally provide a description, start/end times, and event type (live, replay, or on-demand).

**Q: How do I send replays to attendees?**
Use the send_replay action with the webinar ID. This will automatically email the replay link to everyone who attended the completed event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/livestorm](https://vinkius.com/mcp/livestorm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Livestorm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `livestorm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Livestorm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "livestorm": {
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

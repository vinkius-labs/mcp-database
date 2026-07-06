# ON24 Virtual Events MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/on24-virtual-events)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Manage webinars and virtual events via ON24 — track registrants, attendees, and analytics directly from your AI agent.

## Description
Connect your **ON24** account to your AI agent and gain deep insights into your webinar and virtual event performance through natural conversation and real-time data access.

### What you can do

- **Event Oversight** — List all upcoming and past webinars and retrieve detailed scheduling and configuration metadata.
- **Registrant Tracking** — Access complete lists of individuals who have registered for specific events and check their profile details.
- **Attendee Analytics** — Monitor who actually attended your events and retrieve granular engagement and viewing time metrics.
- **Engagement Intelligence** — Access results from event surveys and polls to understand audience sentiment.
- **Q&A Monitoring** — List all questions asked by attendees and their respective answers during live sessions.
- **Performance Reporting** — Fetch high-level event analytics including total views, conversions, and impact scores.
- **Deep Inspection** — Fetch complete metadata for specific events, registrants, or surveys using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your ON24 Client ID, API Key, and API Secret
3. Start managing your virtual event intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Event Marketers** — quickly check registration counts or attendee engagement without opening the ON24 portal.
- **Demand Generation Teams** — monitor event-driven leads and conversion metrics in real-time.
- **Marketing Operations** — automate the retrieval of survey results and Q&A logs for post-event reporting.


## Available Tools (10)
- **get_survey_responses**: Get survey response data
- **list_virtual_events**: List all virtual events
- **get_event_qa_log**: Get event Q&A log
- **list_event_registrants**: List event registrants
- **list_event_surveys**: List event surveys
- **get_event_summary_analytics**: Get event performance summary
- **get_attendee_engagement**: Get attendee engagement stats
- **get_event_details**: Get specific event info
- **get_registrant_details**: Get registrant info
- **list_event_attendees**: List event attendees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ON24 Virtual Events** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my webinars from last month."

**🤖 AI Agent:**
> Retrieving webinars... I found 4 events from last month including 'Product Strategy Q1', 'Customer Onboarding Workshop', and 2 others. Would you like the registration summary for the Product Strategy webinar?

---

**👤 You:**
> "How many people attended the 'Annual Summit' event?"

**🤖 AI Agent:**
> Checking attendance records... For the 'Annual Summit' (ID: 98765), you had 450 total attendees out of 620 registrants (72% attendance rate). Shall I list the engagement metrics for the top attendees?

---

**👤 You:**
> "Show me the survey results for the 'Developer Workshop' webinar."

**🤖 AI Agent:**
> Retrieving survey data... For the 'Developer Workshop' survey, you received 85 responses. The average satisfaction score was 4.7/5. Key feedback included 'Great technical depth' and 'Clear examples'. Would you like the detailed Q&A log as well?


## ❓ FAQ

**Q: How do I get my ON24 API credentials?**
Log in to your ON24 account and navigate to the API Management section in the Analytics or Integration menu to generate your Client ID, API Key, and Secret.

**Q: Can I see attendee viewing time?**
Yes! Use the `get_attendee_engagement` tool with the event ID and attendee email to retrieve detailed engagement metrics including total minutes watched.

**Q: Does this support multi-registration tracking?**
Yes, you can list registrants for any specific event using `list_event_registrants` and check individual registration statuses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/on24-virtual-events](https://vinkius.com/mcp/on24-virtual-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ON24 Virtual Events** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `on24-virtual-events` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ON24 Virtual Events** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "on24-virtual-events": {
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

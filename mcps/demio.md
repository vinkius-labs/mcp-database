# Demio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/demio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Equip your AI agent to manage webinar events, track registrants, and monitor sessions via the Demio API.

## Description
Integrate **Demio**, the modern webinar platform built for marketing, directly into your AI workflow. Manage your upcoming and past webinars, track registration lists, monitor live and scheduled sessions, and register new users using natural language.

### What you can do

- **Webinar Oversight** — List and retrieve detailed settings for all your webinars and check their current status.
- **Registrant Tracking** — List and search through people who have registered for your webinar events.
- **Session Monitoring** — Track scheduled sessions, access attendee lists, and monitor overall session progress.
- **User Registration** — Register new users for specific webinar sessions directly via chat.

### How it works

1. Connect the Demio integration to your AI assistant.
2. Authorize using your Demio API Key and API Secret (found in your account settings).
3. Optimize your webinar marketing strategy through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check registration numbers and session details on the go.
- **Customer Success Teams** — Access registrant info and session status during customer meetings.
- **Event Coordinators** — Manage webinar lists and register participants via chat instantly.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and limits for your Demio account
- **get_webinar_details**: Get detailed settings and information for a specific webinar
- **get_webinar_report**: Retrieve performance metrics and attendance reports for a webinar
- **get_session_details**: Get specific details for a webinar session, including attendees
- **list_webinar_events**: List all upcoming and past webinars in your Demio account
- **list_webinar_registrants**: List all people who have registered for a specific webinar
- **list_webinar_sessions**: List all scheduled sessions for a specific webinar event
- **list_upcoming_webinars**: Identify webinars scheduled for the future
- **register_user_for_webinar**: Register a new user for a specific webinar session
- **search_webinars_by_name**: Search for a webinar using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Demio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming webinars."

**🤖 AI Agent:**
> I've found 3 upcoming webinars: 'Product Demo - New Features', 'Q3 Sales Strategy', and 'Client Onboarding Workshop'. Would you like to see the registration counts for any of these?

---

**👤 You:**
> "Who is registered for the 'Product Demo' webinar?"

**🤖 AI Agent:**
> There are currently 45 people registered for 'Product Demo'. Some notable registrants include 'Alice Johnson' (alice@example.com) and 'Bob Miller' (bob@example.com). Should I search for a specific person?

---

**👤 You:**
> "Show me the report for my last webinar session."

**🤖 AI Agent:**
> Your last session 'Marketing 101' had 120 attendees out of 150 registrants (80% attendance rate). The average time in the session was 45 minutes. Would you like a list of attendees who stayed until the end?


## ❓ FAQ

**Q: How do I get Demio API credentials?**
Log in to your Demio account, navigate to **Settings > API**, and you can retrieve your API Key and API Secret from that section.

**Q: Can the agent see attendance reports?**
Yes, you can use the get_webinar_report tool to retrieve performance metrics and participation data for your webinar events.

**Q: Does the integration support user registration?**
Yes, you can register new users for specific webinar sessions using the register_user_for_webinar action tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/demio](https://vinkius.com/mcp/demio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Demio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `demio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Demio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "demio": {
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

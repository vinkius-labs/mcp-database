# Cronofy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cronofy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling via Cronofy — unify Google, iCloud, and Exchange calendars to manage events and track multi-user availability directly from any AI agent.

## Description
Connect your **Cronofy** account to any AI agent and take full control of your unified calendar and scheduling workflows through natural conversation.

### What you can do

- **Unified Event Management** — List, retrieve, and create events across aggregated Google, iCloud, and Exchange overlays limitlessly
- **Multi-User Availability** — Query availability for up to 10 participants simultaneously, calculating strict intersections to find the perfect meeting time
- **Free/Busy Auditing** — Execute bulk iterations to map time matrices and return exact available boundaries without exposing event payloads
- **Automated Scheduling** — Generate live-availability links and shared scheduling requests to simplify meeting coordination with external members
- **Identity & Profile Mapping** — Inspect unified account canonical IDs and list distinct identity providers connected natively to your Cronofy profile
- **Sync Control** — Irreversibly vaporize explicit validations and delete events to maintain absolute consistency across all connected upstream providers

### How it works

1. Subscribe to this server
2. Enter your Cronofy Access Token (obtained via OAuth flow at app.cronofy.com)
3. Start managing your unified calendars from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Builders** — embed calendar and scheduling automation into AI-powered tools and applications
- **Recruiters & Sales Ops** — coordinate multi-participant meetings and verify availability across different providers in real-time
- **Executive Assistants** — manage complex schedules and generate scheduling links using natural language
- **DevOps Teams** — monitor calendar sync states and audit organizational scheduling requests


## Available Tools (10)
- **read_events**: cronofy.com/v1/events` pulling unified aggregated Google, iCloud, and Exchange overlays limitlessly.

Identify bounded CRM records inside the Headless Cronofy Engine
- **create_event**: Provision a highly-available JSON Payload generating explicit Sync links
- **delete_event**: Irreversibly vaporize explicit validations extracting rich Provider syncs
- **list_calendars**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly
- **get_free_busy**: Enumerate explicitly attached structured rules exporting active Overlaps
- **query_availability**: Dispatch an automated validation check routing explicit Cross-Provider checks
- **get_account**: Inspect deep internal arrays mitigating specific Sub Provider lists
- **get_user_info**: Identify precise active arrays spanning native Gateway auth bounds
- **list_profiles**: Retrieve the exact structural matching verifying Blueprint directories
- **create_scheduling_request**: Fetch elaborate explicit mapped limits via native forms dispatch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cronofy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my calendar events from tomorrow to next week"

**🤖 AI Agent:**
> Retrieving unified events... I found 8 events across your Google and Exchange calendars. Highlights include 'Client Kickoff' on Tuesday at 10 AM and 'Team Sync' on Thursday at 2 PM.

---

**👤 You:**
> "Find a 30-minute slot for a meeting with john@example.com tomorrow"

**🤖 AI Agent:**
> Analyzing availability... John has three 30-minute slots available tomorrow: 9:30 AM, 1:00 PM, and 4:30 PM. Which one works best for you?

---

**👤 You:**
> "Create a scheduling link for a 'Project Review' meeting"

**🤖 AI Agent:**
> Scheduling request created! Here is the link for the 'Project Review': https://scheduling.cronofy.com/r/abc-123. This link is mapped to your live availability across all connected calendars.


## ❓ FAQ

**Q: Can my agent check availability across different calendar providers like Google and iCloud?**
Yes. Use the 'query_availability' tool. Your agent will traverse multi-user JSON payloads and calculate strict intersections across all connected accounts, regardless of the underlying calendar provider.

**Q: How do I create a new calendar event via the agent?**
Provide the 'calendar_id', 'summary', and 'start/end' times to the 'create_event' tool. The agent commands Cronofy to update your upstream provider synchronously, ensuring the event appears on your calendar immediately.

**Q: Can I generate a public scheduling link through chat?**
Absolutely. Use the 'create_scheduling_request' tool. The agent will generate a shared UI link mapped to your live availability, which you can then share externally to let others book time with you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cronofy](https://vinkius.com/mcp/cronofy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cronofy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cronofy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cronofy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cronofy": {
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

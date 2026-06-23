# Notion Calendar (formerly Cron) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notion-calendar-formerly-cron)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage scheduling via Notion Calendar — create events, track team availability, and manage scheduling links directly from any AI agent.

## Description
Connect your **Notion Calendar** (formerly Cron) account to any AI agent and take full control of your beautifully designed scheduling workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and retrieve exact CRM records extracting events tied strictly to specific date constraints and Notion sync states
- **Live Scheduling** — Provision highly-available Event payloads generating hard schedule binds synchronized directly to upstream Google or Microsoft logic
- **Availability Auditing** — Dispatch automated validation checks to process cross-calendar math and isolate available bookable limits explicitly
- **Team Coordination** — Enumerate explicitly attached structural rules to analyze `freeBusy` cross-references and predict collision limits across multiple emails
- **Booking Links** — Retrieve precise active scheduling forms and booking links tied directly to your profile settings for instant sharing
- **Profile Management** — Inspect deep internal arrays of your Cron profile, including localized preferences and unified calendar provider connections

### How it works

1. Subscribe to this server
2. Enter your Notion Calendar (Cron) API Key
3. Start managing your calendar and availability from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — create and manage events or check availability without leaving the workspace
- **Teams & Managers** — coordinate meeting times and audit team availability across overlapping calendars
- **Power Users** — integrate their Notion-based scheduling workflows into automated AI agents
- **Operations Teams** — monitor scheduling link status and manage calendar profile settings through natural language


## Available Tools (10)
- **list_events**: Identify bounded CRM records inside the Headless Cron Engine
- **get_event**: Perform structural extraction of properties driving active Event targets
- **create_event**: Provision a highly-available Event Payload generating hard Schedule binds
- **update_event**: Dissect precise variables checking active state matching payload targets
- **delete_event**: Irreversibly vaporize explicit validations extracting rich Schedule drops
- **list_calendars**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly
- **get_availability**: Dispatch an automated validation check routing explicit Availability
- **get_scheduling_links**: Identify precise active arrays spanning native Gateway limits
- **get_free_busy**: Enumerate explicitly attached structured rules exporting active Graph overlaps
- **get_profile**: Inspect deep internal arrays mitigating specific Math Logic limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notion Calendar (formerly Cron)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my calendar events for today"

**🤖 AI Agent:**
> I found 3 events for today: 'Morning Sync' at 9:00 AM, 'Product Review' at 2:00 PM, and 'Team Coffee' at 4:30 PM. Would you like to see the details for any of these?

---

**👤 You:**
> "Check if john@acme.com and sarah@acme.com are free tomorrow"

**🤖 AI Agent:**
> Analyzing schedules for tomorrow... Both John and Sarah are free between 10:00 AM - 11:30 AM and 2:00 PM - 3:00 PM. Would you like me to schedule a meeting in one of these slots?

---

**👤 You:**
> "Give me my booking link for '15 Minute Coffee Chat'"

**🤖 AI Agent:**
> Here is your scheduling link for '15 Minute Coffee Chat': https://cron.com/johndoe/15-min-coffee. This link is active and ready to be shared with your clients.


## ❓ FAQ

**Q: Can my agent create events on my synced Google or Outlook calendars?**
Yes. When you use the 'create_event' tool, the agent commands the Notion Calendar backend to generate the meeting overlay, which is then synchronized directly to your connected upstream provider logic.

**Q: How do I check if my team members are free for a meeting on a specific date?**
Use the 'get_free_busy' tool. Provide a JSON array of email addresses and the target date. Your agent will analyze the cross-references and identify available hourly slots, predicting any potential collision limits.

**Q: Can I retrieve my scheduling links via chat to share with clients?**
Absolutely. The 'get_scheduling_links' tool extracts the precise active booking forms tied directly to your Notion Calendar profile, allowing your agent to provide you with ready-to-share links instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion-calendar-formerly-cron](https://vinkius.com/mcp/notion-calendar-formerly-cron)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Notion Calendar (formerly Cron)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `notion-calendar-formerly-cron` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Notion Calendar (formerly Cron)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "notion-calendar-formerly-cron": {
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

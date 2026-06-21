# Guidebook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidebook-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create branded mobile apps for events, conferences, and organizations with schedules, maps, and attendee engagement features.

## Description
Connect your **Guidebook Builder** account to any AI agent and take full control of your mobile event guides and scheduling workflows through natural conversation.

### What you can do

- **Guide Orchestration** — List and manage all mobile guides in your account and retrieve detailed guide metadata
- **Schedule Management** — Access and monitor event schedules and sessions programmatically to keep your attendees updated
- **Location Mapping** — List and search for mapped event locations to ensure precise spatial coordination for your attendees
- **Custom Lists** — Manage and retrieve custom lists (speakers, exhibitors, sponsors) to organize your event's intellectual capital
- **Activity Monitoring** — Check guide details and status directly through your agent for instant event reporting

### How it works

1. Subscribe to this server
2. Retrieve your API Key from the Guidebook Builder (Manage your account > API Key)
3. Start managing your mobile guides from Claude, Cursor, or any MCP client

No more manual editing of sessions or locations through complex web builders. Your AI acts as your dedicated event mobile coordinator.

### Who is this for?

- **Event Organizers** — scale mobile guide management and session coordination for large-scale conferences
- **Marketing Teams** — update exhibitor and sponsor lists across multiple guides through natural language queries
- **Onboarding Leads** — keep employees updated on company training schedules and locations without leaving your workspace


## Available Tools
- **check_guidebook_status**: Verify connectivity
- **create_custom_list_item**: Add list item
- **create_guide**: Create a guide
- **get_event**: Get session details
- **get_guide**: Get guide details
- **list_attendees**: List attendees
- **list_custom_list_items**: List custom list items
- **list_custom_lists**: List custom lists
- **list_events**: List sessions
- **list_guides**: List guides
- **list_locations**: List locations
- **update_guide**: Update a guide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guidebook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my mobile guides in Guidebook."

**🤖 AI Agent:**
> I've retrieved your mobile guides. You have 3 active guides: 'Global Tech Expo 2026' (ID: g_123), 'Internal Sales Kickoff' (ID: g_456), and 'Partner Summit' (ID: g_789). Which one would you like to inspect?

---

**👤 You:**
> "Show the schedule for the 'Global Tech Expo 2026' guide."

**🤖 AI Agent:**
> Fetching schedule for Global Tech Expo (ID: g_123)... I found 12 scheduled sessions. Notable highlights include 'AI in Industry' at 10 AM and the 'Cloud Keynote' at 2 PM. Would you like the location details for any of these?

---

**👤 You:**
> "List all speakers for the guide ID 'g_123'."

**🤖 AI Agent:**
> Scanning custom lists for 'g_123'... I've retrieved the speaker list. You have 25 speakers registered, including keynote presenters and technical leads. I can provide the full list or search for a specific name.


## ❓ FAQ

**Q: How do I find a Guide ID?**
You can use the `list_guides` tool to retrieve all mobile guides in your account along with their unique identifiers and names.

**Q: Can I see the speakers or exhibitors for an event?**
Yes! Use the `list_custom_lists` tool with a specific `guide_id` to retrieve all custom directories like speakers, exhibitors, or sponsors.

**Q: Does the integration support viewing the event map?**
The `list_guide_locations` tool provides the metadata for all mapped locations within a guide, helping you identify precisely where sessions take place.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidebook-alternative](https://vinkius.com/mcp/guidebook-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guidebook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `guidebook-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guidebook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guidebook-alternative": {
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

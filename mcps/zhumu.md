# Zhumu / 瞩目 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zhumu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Leading video conferencing platform in China — manage meetings, users, and recordings via AI.

## Description
Empower your AI agent to orchestrate your video collaboration with **Zhumu** (瞩目), the premier cloud meeting platform in China. By connecting Zhumu to your agent, you transform complex meeting scheduling, user auditing, and recording management into a natural conversation. Your agent can instantly list upcoming meetings, retrieve detailed participant information, monitor cloud recordings, and even schedule new sessions without you ever needing to navigate the comprehensive Zhumu portal. Whether you are conducting a cross-functional team sync or coordinating a large-scale webinar, your agent acts as a real-time collaboration assistant, keeping your schedule accurate and your meetings organized.

### What you can do

- **Meeting Orchestration** — List, retrieve, and schedule video meetings with full support for topics and timing.
- **User Auditing** — Browse and retrieve detailed user profiles across your organization.
- **Recording Control** — List and access cloud recordings for past sessions to ensure knowledge sharing.
- **Webinar Monitoring** — Monitor scheduled webinars and participant engagement levels.
- **Usage Insights** — Retrieve high-level account reports and activity summaries for your collaboration environment.

### How it works

1. Subscribe to this server
2. Enter your Zhumu App Key and App Secret
3. Start managing your video collaboration through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor team syncs and coordinate meeting schedules through natural language queries.
- **HR & Operations** — manage user accounts and monitor organization-wide usage directly from your AI-powered workspace.
- **Event Coordinators** — oversee webinars and retrieve recording metadata via a unified AI interface.
- **Zhumu Power Users** — integrate your existing meeting workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_account_report**: Get usage reports
- **get_meeting**: Get meeting details
- **get_user**: Get user details
- **list_meetings**: List upcoming meetings
- **list_recordings**: List cloud recordings
- **list_users**: List organization users
- **list_webinars**: List scheduled webinars
- **update_meeting**: Update meeting settings
- **create_meeting**: Create a new meeting
- **delete_meeting**: Delete a meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zhumu / 瞩目** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming meetings in Zhumu."

**🤖 AI Agent:**
> I've retrieved your upcoming meetings. You have 3 sessions scheduled for today, including 'Weekly Sync' and 'Product Review'. Would you like the dial-in details for the next one?

---

**👤 You:**
> "Schedule a meeting titled 'Design Feedback' for today."

**🤖 AI Agent:**
> Done! I've scheduled your 'Design Feedback' meeting. The meeting ID is '8821' and it has been added to your calendar. Should I send the invite to the participants?

---

**👤 You:**
> "Show me the last 5 cloud recordings."

**🤖 AI Agent:**
> I've listed your 5 most recent recordings. The largest is 'Project Launch' from yesterday. Would you like the download links or the access passwords for these files?


## ❓ FAQ

**Q: How do I find my Zhumu App Key and Secret?**
Log in to the Zhumu Developer Center, create a new application, and you will find your unique App Key and App Secret in the application credentials section.

**Q: Can I retrieve meeting recordings through this server?**
Yes. Use the `list_recordings` tool with a specific user ID to retrieve a list of all cloud recordings saved for that user's sessions.

**Q: Is it possible to manage webinars?**
Yes! Use the `list_webinars` tool to retrieve a list of all scheduled webinars and identify upcoming sessions and engagement metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zhumu](https://vinkius.com/mcp/zhumu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zhumu / 瞩目** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zhumu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zhumu / 瞩目** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zhumu": {
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

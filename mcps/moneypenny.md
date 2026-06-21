# Moneypenny MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moneypenny)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Never miss a business call with dedicated virtual receptionists and live chat agents who represent your brand professionally.

## Description
Connect your **Moneypenny** account to any AI agent and review your business communications through natural conversation.

### What you can do

- **Call Messages** — Browse telephone answering messages by day, week, month, or custom date range.
- **Live Chat Logs** — Access live chat conversation transcripts with time-based filtering.
- **Activity Summary** — Get a combined overview of today's calls and chats in a single dashboard view.
- **Time-Based Views** — Instantly access today's, this week's, or this month's communications.

### How it works

1. Subscribe to this server
2. Enter your Moneypenny portal credentials
3. Start reviewing communications from Claude, Cursor, or any MCP client

### Who is this for?

- **Business Owners** — review call summaries and chat activity without logging into the portal.
- **Office Managers** — monitor receptionist performance and communication volume.
- **Customer Service Leads** — track response patterns and interaction trends.


## Available Tools
- **get_activity_summary**: Get a summary of all calls and chats for today
- **list_call_messages**: Format dates as MM/DD/YYYY.

List telephone answering messages by date range
- **list_chat_logs**: Optionally filter by start and end time (ISO 8601).

List live chat conversation logs by date range
- **get_this_month_calls**: Get all call messages from the current month
- **get_recent_chats**: Returns all new chat conversations.

Get the most recent live chat conversations
- **check_moneypenny_status**: Verify Moneypenny API connectivity
- **get_today_calls**: Get all call messages from today
- **get_today_chats**: Get all live chat conversations from today
- **get_this_week_calls**: Get all call messages from the past 7 days
- **get_this_week_chats**: Get all live chat conversations from the past 7 days


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moneypenny** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's call messages."

**🤖 AI Agent:**
> You received 8 call messages today. The most recent was from James Wilson at 3:45 PM regarding a project quote request. 3 calls were marked as urgent. Would you like to see the full details?

---

**👤 You:**
> "Give me a summary of today's activity."

**🤖 AI Agent:**
> Today's activity summary: 8 telephone messages and 12 live chat conversations, totaling 20 interactions handled by your Moneypenny team.

---

**👤 You:**
> "Show me the live chat logs from this week."

**🤖 AI Agent:**
> You had 47 live chat conversations this week. Peak activity was on Tuesday with 14 chats. The average response time was under 30 seconds. Would you like details for a specific day?


## ❓ FAQ

**Q: How do I quickly check today's call activity?**
Use the `get_today_calls` tool for an instant view of all telephone messages received today, or `get_activity_summary` for a combined call and chat count.

**Q: Can I see chat conversations from the last week?**
Yes! Use `get_this_week_chats` for a 7-day overview, or `list_chat_logs` with custom start and end times for any date range.

**Q: What authentication does Moneypenny require?**
Moneypenny uses your portal email and password to generate a Bearer token automatically. The token refreshes every 24 hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moneypenny](https://vinkius.com/mcp/moneypenny)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moneypenny** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moneypenny` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moneypenny** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moneypenny": {
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

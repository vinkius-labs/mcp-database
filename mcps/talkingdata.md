# TalkingData MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/talkingdata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Leading big data and product analytics platform in China — manage event tracking and user growth via AI.

## Description
Empower your AI agent to orchestrate your product intelligence and user behavioral data with **TalkingData**, the premier big data platform in China. By connecting TalkingData to your agent, you transform complex event tracking auditing, user growth analysis, and multi-channel attribution into a natural conversation. Your agent can instantly retrieve high-level application summaries, monitor active user trends, audit custom event data, and even provide detailed hardware device statistics without you ever needing to navigate the comprehensive TalkingData portal. Whether you are conducting a product health audit or monitoring real-time campaign performance across different channels, your agent acts as a real-time data analyst assistant, keeping your metrics accurate and your growth moving.

### What you can do

- **Metrics Orchestration** — Retrieve real-time active user, new registration, and retention statistics for your application.
- **Event Auditing** — Browse tracked custom events and retrieve detailed analytical data for specific behavioral triggers.
- **Channel Monitoring** — Analyze user acquisition and performance across different marketing and distribution channels.
- **Hardware Insights** — Access detailed breakdowns of user devices, including model, OS, and hardware specifications.
- **Session Analysis** — Retrieve average session duration and usage frequency to monitor product engagement levels.

### How it works

1. Subscribe to this server
2. Enter your TalkingData App ID and API Key (Access Token)
3. Start managing your product analytics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor feature adoption and audit user behavior through natural language queries.
- **Data Analysts** — retrieve system-wide behavioral metrics and perform cohort analysis via a unified AI interface.
- **Growth Engineers** — coordinate channel performance and monitor user retention directly from your AI-powered workspace.
- **TalkingData Power Users** — integrate your existing big data workflows into your AI-driven daily routines.


## Available Tools
- **get_active_users**: Get active user statistics
- **get_app_info**: Get application configuration info
- **get_app_summary**: Get application performance summary
- **get_channel_data**: Get acquisition channel data
- **get_device_stats**: Get device hardware statistics
- **get_event_data**: Get custom event analytics
- **get_new_users**: Get new user registrations
- **get_session_stats**: Get session usage statistics
- **get_user_retention**: Get user retention data
- **list_events**: List tracked events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TalkingData** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the application performance summary."

**🤖 AI Agent:**
> I've retrieved your TalkingData application summary. You currently have 50,000 total users with a 12% growth rate this month. Your most active region is East China. Should I check the retention metrics for your newest cohort?

---

**👤 You:**
> "What is the active user count for today?"

**🤖 AI Agent:**
> Your active user count for today is 12,500, which is 8% higher than yesterday at this same time. Would you like a breakdown of these users by acquisition channel?

---

**👤 You:**
> "List all tracked events in the app."

**🤖 AI Agent:**
> I've listed your tracked events. There are 25 custom events currently active, including 'Registration_Complete', 'Add_to_Cart', and 'Level_Up'. Which event would you like to see detailed analytics for?


## ❓ FAQ

**Q: How do I find my TalkingData App ID and API Key?**
Log in to the [TalkingData portal](https://www.talkingdata.com/), select your application from the management console, and you will find your AppID and API Key (Access Token) in the application settings or 'App Info' section.

**Q: Can I query data for a specific date range?**
Yes. Tools like `get_active_users` and `get_new_users` accept optional `start_date` and `end_date` parameters (in YYYY-MM-DD format) to retrieve statistics for specific periods.

**Q: Is it possible to list all custom events?**
Yes! Use the `list_events` tool to retrieve a complete list of all custom behavioral events currently being tracked in your application, along with their unique identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/talkingdata](https://vinkius.com/mcp/talkingdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TalkingData** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `talkingdata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TalkingData** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "talkingdata": {
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

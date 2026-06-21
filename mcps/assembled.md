# Assembled MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assembled)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage support workforce and scheduling with Assembled — track agent states, teams, and forecasts via AI.

## Description
The **Assembled MCP Server** provides your AI agent with direct access to your workforce management (WFM) data. Optimize your support operations by monitoring agent availability, auditing schedules, and analyzing contact volume forecasts using natural language.

### Key Capabilities

- **Agent & State Tracking** — List all users and monitor real-time agent states to see who is online, on break, or in a meeting.
- **Team & Queue Management** — Audit your support organization structure by listing teams and individual support queues.
- **Schedule Oversight** — Retrieve detailed agent schedules for any time range to ensure proper coverage.
- **Forecasting Insights** — Access contact volume forecasts to prepare for upcoming support demand.
- **Operational Auditing** — Quickly verify account connections and organizational metadata without manual reports.
- **Secure API Access** — Uses your Assembled API Key for safe and authenticated communication with your WFM data.

### Who is this for?

- **Support Managers** — Quickly check team coverage and agent statuses during busy periods.
- **Workforce Analysts** — Retrieve schedule and forecast data for planning and optimization.
- **Operations Leads** — Monitor real-time agent states and queue health using simple natural language commands.


## Available Tools
- **get_account_check**: Verify Assembled account connection
- **list_agent_states**: List real-time agent states
- **list_forecasts**: List contact volume forecasts
- **list_queues**: List all support queues
- **list_schedules**: List agent schedules for a time range
- **list_teams**: List all teams
- **list_users**: List all users in Assembled


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assembled** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all agents currently online in Assembled."

**🤖 AI Agent:**
> I've retrieved the current agent states. You have 15 agents online, 3 on lunch, and 2 in a training session.

---

**👤 You:**
> "Show me the schedule for 'Support Team Alpha' for today."

**🤖 AI Agent:**
> I've pulled the schedule for Team Alpha. Coverage looks good until 4:00 PM, with a slight dip during the 12:00 PM lunch rotation.

---

**👤 You:**
> "What is the contact volume forecast for next Monday?"

**🤖 AI Agent:**
> The forecast for next Monday predicts a peak of 250 tickets per hour between 10:00 AM and 12:00 PM UTC.


## ❓ FAQ

**Q: How do I get my Assembled API Key?**
Log in to your Assembled account, go to **Settings > API Keys**, and you can generate a new API key there.

**Q: Can I see who is currently on break?**
Yes, use the `list_agent_states` tool to see the real-time status of all your agents, including those on breaks or in specific states.

**Q: How far in advance can I see schedules?**
You can retrieve schedules for any time range by providing the `startTime` and `endTime` parameters to the `list_schedules` tool, as long as they are published in Assembled.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assembled](https://vinkius.com/mcp/assembled)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assembled** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `assembled` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assembled** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assembled": {
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

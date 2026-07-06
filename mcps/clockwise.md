# Clockwise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clockwise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling via Clockwise — manage focus time, track team availability, and optimize calendar events directly from any AI agent.

## Description
Connect your **Clockwise** account to any AI agent and take full control of your intelligent calendar workflows through natural conversation.

### What you can do

- **Focus Time Management** — List and audit AI-created focus time blocks to ensure you have space for deep work
- **Team Availability** — Check overlapping free windows across multiple team members to find the perfect meeting time
- **Calendar Optimization** — Monitor flexible events and toggle Autopilot to let AI intelligently move meetings for optimal productivity
- **Meeting Analytics** — Retrieve historical data on meeting fragmentation and context switching costs
- **Time Insights** — Get weekly or monthly reports on deep work achievements and calendar health
- **Preference Control** — Audit and update meeting-free days, lunch breaks, and focus time goals directly from your workspace

### How it works

1. Subscribe to this server
2. Enter your Clockwise API Key or OAuth Token
3. Start managing your intelligent calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — protect focus time and manage calendar preferences without manual adjustments
- **Team Leads** — audit collective availability and optimize meeting schedules for the entire squad
- **Operations Managers** — analyze time insights and fragmentation costs to improve organizational productivity
- **Developers** — integrate calendar health checks and focus time monitoring into your dev workflow


## Available Tools (10)
- **get_preferences**: Retrieve the exact structural matching verifying explicit user settings
- **get_calendar_events**: Identify bounded logical arrays managing top-level calendar blocks
- **get_focus_time**: Perform structural extraction of properties driving active Deep Work limits
- **update_preferences**: Provision a highly-available override payload updating Clockwise configurations
- **get_team_availability**: Identify explicit Cloud calculations tracking absolute team free times
- **get_autopilot_status**: Extracts explicitly attached internal structural states pulling logic engine mappings
- **toggle_autopilot**: Irreversibly mutate explicit boundaries toggling intelligent meeting moving
- **get_meeting_analytics**: Identify precise active arrays spanning meeting metadata histories
- **get_time_insights**: Extracts structural arrays resolving AI-nested focus analytics
- **get_current_user**: Retrieve the root identity mappings bounding specific organization accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clockwise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my team's availability for tomorrow? Emails: ['john@acme.com', 'sarah@acme.com']"

**🤖 AI Agent:**
> Analyzing availability... Both John and Sarah are free between 10:00 AM - 11:30 AM and 2:00 PM - 3:30 PM tomorrow. Would you like me to schedule a meeting in one of these slots?

---

**👤 You:**
> "Show me my focus time insights for this month"

**🤖 AI Agent:**
> This month, you achieved 45 hours of deep work across 22 Focus Time blocks. Your calendar fragmentation decreased by 12% compared to last month. Great job!

---

**👤 You:**
> "Set my focus time goal to 3 hours per day"

**🤖 AI Agent:**
> Preferences updated! Your focus time goal is now set to 3 hours per day. Clockwise Autopilot will begin adjusting your flexible meetings to meet this target.


## ❓ FAQ

**Q: Can my agent protect my Focus Time automatically?**
Yes. Use the 'update_preferences' tool to set your focus time goals. The Clockwise AI will then automatically identify and block space on your calendar, and your agent can monitor these blocks using the 'get_focus_time' tool.

**Q: How do I find a common meeting time for several teammates?**
Provide your agent with a list of emails and a target date. The 'get_team_availability' tool will aggregate free windows across all specified calendars, allowing the agent to suggest the best time for everyone.

**Q: Is Clockwise really shutting down in 2026?**
Yes, the Clockwise team is joining Salesforce, and the service is scheduled to sunset on March 27, 2026. Users are encouraged to migrate to alternative solutions like Reclaim.ai before this date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clockwise](https://vinkius.com/mcp/clockwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clockwise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clockwise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clockwise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clockwise": {
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

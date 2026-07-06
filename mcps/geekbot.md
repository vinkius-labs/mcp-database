# Geekbot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geekbot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Run asynchronous standups and team check-ins through Slack or Microsoft Teams that respect everyone timezone and schedule.

## Description
Connect your **Geekbot** account to any AI agent and take full control of your team's standups, surveys, and reporting workflows through natural conversation.

### What you can do

- **Standup Orchestration** — List and retrieve detailed metadata for all configured standups and polls in your workspace programmatically
- **Report Intelligence** — Monitor user responses in real-time and retrieve complete answer histories for analysis and sentiment tracking
- **Report Automation** — Programmatically submit standup reports on behalf of users or fetch granular data for specific time periods
- **Team Visibility** — Access your complete workspace directory to manage member roles and understand team-wide participation
- **Activity Monitoring** — Check account status and individual user profiles directly through your agent for instant team reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Geekbot settings (Settings > Developers)
3. Start managing your team coordination from Claude, Cursor, or any MCP client

No more manual checking of Slack channels for missing standups. Your AI acts as your dedicated team operations assistant.

### Who is this for?

- **Project Managers** — instantly retrieve standup summaries and identify blockers using natural language queries
- **Team Leads** — monitor team sentiment and participation rates without leaving your communication tools
- **HR & Ops** — automate the collection of team feedback and internal surveys through simple AI commands


## Available Tools (6)
- **list_standups**: List your Geekbot standups
- **list_team_members**: List workspace members
- **submit_standup_report**: Programmatically submit a report
- **get_user_profile**: Check account connection
- **get_standup_details**: Get metadata for a standup
- **list_standup_reports**: Can filter by date or user.

List submitted reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geekbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active standups in my Geekbot account."

**🤖 AI Agent:**
> I've retrieved your standups. You have 3 active configurations: 'Daily Standup' (ID: std_1), 'Friday Retrospective' (ID: std_2), and 'Monthly Poll' (ID: std_3). Which one should we review?

---

**👤 You:**
> "Show me the reports for 'Daily Standup' from the last 24 hours."

**🤖 AI Agent:**
> Scanning responses for 'Daily Standup'... I found 8 reports submitted today. Most members are focused on 'API Documentation' and 'Frontend Cleanup'. There are 2 reported blockers. Would you like to see the details of the blockers?

---

**👤 You:**
> "List all members in our Geekbot workspace."

**🤖 AI Agent:**
> Fetching member directory... You have 15 members in your workspace. Notable users include 'Alice' (Admin), 'Bob' (Developer), and 'Charlie' (Designer). I can provide their individual IDs or participation history if needed.


## ❓ FAQ

**Q: How do I find my Geekbot API Key?**
Log in to your Geekbot dashboard, navigate to **Settings** > **Developers**, and copy your unique API Key.

**Q: Can I filter standup reports by user?**
Yes! The `list_standup_reports` tool accepts a `user_id` parameter to retrieve responses for a specific team member.

**Q: How do I get a member's User ID?**
Use the `list_team_members` tool to retrieve a directory of everyone in your workspace along with their unique Geekbot IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geekbot](https://vinkius.com/mcp/geekbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geekbot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geekbot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geekbot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geekbot": {
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

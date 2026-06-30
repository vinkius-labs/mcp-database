# Range MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/range)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Keep distributed teams in sync with async check-ins, team updates, and meeting tools that reduce unnecessary status meetings.

## Description
Connect your **Range.co** account to any AI agent and take full control of your team communication and check-in orchestration through natural conversation. Range provides a premier platform for keeping remote and hybrid teams synchronized, and this integration allows you to retrieve team metadata, monitor check-in updates (snippets), and track organizational objectives directly from your chat interface.

### What you can do

- **Check-in & Update Orchestration** — List all managed updates and retrieve detailed metadata including snippet content programmatically.
- **Team & User Lifecycle Management** — Access and monitor your workspace teams and retrieve detailed user profile metadata directly from the AI interface.
- **Objective & Goal Intelligence** — Access organizational objectives to maintain a clear overview of team alignment and progress via natural language.
- **Activity & Snippet Control** — Retrieve specific snippets and check-in details to stay informed about daily team accomplishments.
- **Operational Monitoring** — Track system activity and manage workspace metadata using simple AI commands to ensure your team remains high-performing.

### How it works

1. Subscribe to this server
2. Enter your Range API Key from your developer settings
3. Start managing your team check-ins from Claude, Cursor, or any MCP-compatible client

No more manual check-in reading or missed status updates. Your AI acts as a dedicated operations manager or team coordinator.

### Who is this for?

- **Engineering Managers** — quickly retrieve daily updates and monitor team progress without switching apps.
- **Product Leads** — automate the retrieval of objective statuses and track feature delivery via natural conversation.
- **Operations Teams** — streamline the retrieval of user metadata and monitor organizational health directly within the chat.


## Available Tools (11)
- **get_user**: Get details for a specific team member
- **list_goals**: List all team goals
- **list_objectives**: List team objectives
- **list_teams**: List all teams
- **list_updates**: Can be filtered by target_id or for_user_id.

List team check-ins (updates)
- **list_users**: List all users in the organization
- **create_update**: Post a new standup update
- **get_objective**: Get details for a specific objective
- **get_snippet**: Get details of a specific check-in snippet
- **get_team**: Get details for a specific team
- **get_update**: Get details of a specific update (check-in)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Range** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all teams in my Range workspace."

**🤖 AI Agent:**
> I've retrieved your teams. You have 3 active groups: 'Product Team', 'Infrastructure', and 'Marketing Hub'. Which one would you like to see member updates for?

---

**👤 You:**
> "Show me all team standup updates from today with their mood indicators and blockers."

**🤖 AI Agent:**
> 8 of 12 team members posted updates today. Mood average: 3.8/5 (good). Highlights: Sarah completed the API redesign (3 objectives linked). James shipped the mobile notification feature. 3 blockers reported: "Waiting on design assets" (Alex, 2 days blocked), "Staging environment down" (Lisa, since morning), "Third-party API rate limit" (Mike, intermittent). 4 team members have not posted yet. Yesterday's unresolved blockers: 1 resolved, 2 carried over.

---

**👤 You:**
> "Show me the progress on all team objectives for this quarter with completion percentages."

**🤖 AI Agent:**
> 5 team objectives for Q2. "Launch Mobile App v2" at 78% (on track, 6 of 8 milestones complete). "Reduce Customer Churn" at 65% (slightly behind, churn down from 5.2% to 4.1%, target: 3.5%). "API Response Time < 200ms" at 92% (ahead of schedule, current avg: 187ms). "Onboard 50 Enterprise Clients" at 56% (28 onboarded, pace needs acceleration). "Complete SOC 2 Certification" at 85% (final audit scheduled May 28). Overall Q2 objective health: 75.2%.


## ❓ FAQ

**Q: Can my AI automatically find the recent check-ins for a specific user?**
Yes! Use the `list_updates` tool with the `for_user_id` parameter. Your agent will respond with the most recent check-in snippets and status updates in seconds.

**Q: How do I find my Range API Key?**
Log in to Range, go to **Settings** > **Developer Settings** > **API Keys**, and generate a new key for your account.

**Q: Can I see team objectives via the AI?**
Yes, use the `list_objectives` tool to retrieve all active goals and targets configured in your Range workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/range](https://vinkius.com/mcp/range)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Range** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `range` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Range** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "range": {
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

# Range MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/range)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/range-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/range-mcp)
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


## Available Tools
- **create_update**: Post a new standup update
- **get_objective**: Get details for a specific objective
- **get_snippet**: Get details of a specific check-in snippet
- **get_team**: Get details for a specific team
- **get_update**: Get details of a specific update (check-in)
- **get_user**: Get details for a specific team member
- **list_goals**: List all team goals
- **list_objectives**: List team objectives
- **list_teams**: List all teams
- **list_updates**: Can be filtered by target_id or for_user_id.

List team check-ins (updates)
- **list_users**: List all users in the organization


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


## Installation & Usage

To install and use the **Range** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/range](https://vinkius.com/mcp/range)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Assembled MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assembled)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/assembled-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/assembled-mcp)
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


## Installation & Usage

To install and use the **Assembled** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assembled](https://vinkius.com/mcp/assembled)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

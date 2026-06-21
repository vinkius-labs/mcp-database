# Opsgenie MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opsgenie)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opsgenie-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opsgenie-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate incident management via Opsgenie — manage alerts, track on-calls, and coordinate incidents directly from any AI agent.

## Description
Connect your **Opsgenie** account to any AI agent and take full control of your incident response workflows through natural conversation.

### What you can do

- **Alert Management** — Create, acknowledge, and close alerts. Add notes to the activity log to keep the team informed.
- **Incident Coordination** — Create and track major incidents with priority levels to mobilize the right people quickly.
- **On-Call Visibility** — Instantly check who is on-call for any schedule to route issues to the correct responder.
- **Schedule Overview** — List all your on-call schedules and rotations to maintain a clear view of team availability.
- **Query & Audit** — List alerts and incidents using powerful queries to audit past events or find active issues.

### How it works

1. Subscribe to this server
2. Enter your Opsgenie API Key (GenieKey)
3. (Optional) Specify your region (US or EU)
4. Start managing your operations from Claude, Cursor, or any MCP client

### Who is this for?

- **SRE & DevOps Engineers** — quickly acknowledge alerts or add technical notes while investigating issues in your IDE.
- **Incident Managers** — create major incidents and check on-call schedules during high-pressure situations.
- **Support Teams** — verify if there's an active alert for a reported issue and see who is currently handling it.


## Available Tools
- **acknowledge_alert**: Acknowledge an alert
- **add_note**: Add a note to an alert
- **close_alert**: Close an alert
- **create_alert**: Create a new Opsgenie alert
- **create_incident**: Create a new incident
- **get_alert**: Get details for a specific alert
- **get_incident**: Get details for a specific incident
- **get_who_is_on_call**: Get current on-call users for a schedule
- **list_alerts**: List Opsgenie alerts
- **list_incidents**: List Opsgenie incidents
- **list_schedules**: List all on-call schedules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Opsgenie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently open P1 alerts."

**🤖 AI Agent:**
> I've found 3 open P1 alerts. 1. 'Database latency high' (ID: 4930), 2. 'API Gateway 5xx errors' (ID: 4931), 3. 'Payment service down' (ID: 4932).

---

**👤 You:**
> "Acknowledge alert 4930 and add a note saying 'I am investigating the connection pool limits'."

**🤖 AI Agent:**
> Alert 4930 has been acknowledged and the note has been added to the activity log. You are now the owner of this alert.

---

**👤 You:**
> "Who is currently on-call for the 'SRE-Primary' schedule?"

**🤖 AI Agent:**
> The current on-call responder for 'SRE-Primary' is Sarah Miller (sarah.miller@example.com). Her shift ends at 08:00 AM UTC tomorrow.


## Installation & Usage

To install and use the **Opsgenie** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opsgenie](https://vinkius.com/mcp/opsgenie)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

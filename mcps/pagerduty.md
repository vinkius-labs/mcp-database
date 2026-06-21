# PagerDuty MCP Server

Manage incidents, services, on-call schedules, and escalation policies via PagerDuty — trigger, acknowledge, and resolve alerts from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pagerduty)

## Overview
**Category:** industry-titans
**Tools Count:** 11

## Description
Connect your **PagerDuty** account to any AI agent and take full control of incident management operations through natural conversation.

### What you can do

- **Incident Management** — List, create, acknowledge, and resolve incidents across all services
- **Service Monitoring** — Browse all monitored services and inspect their configurations, integrations, and health status
- **User Management** — List all team members, view individual profiles, contact methods, and notification rules
- **On-Call Visibility** — See who is currently on-call across all schedules and escalation levels in real-time
- **Schedule Administration** — Browse rotation schedules with their layers, handoff times, and coverage windows
- **Escalation Policies** — Inspect escalation chains to understand how incidents route through teams

### How it works

1. Subscribe to this server
2. Enter your PagerDuty REST API Key from Configuration > API Access
3. Start managing incidents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SRE Engineers** — quickly triage and resolve incidents without leaving your IDE
- **Engineering Managers** — get instant visibility into active incidents and on-call coverage
- **DevOps Teams** — automate incident workflows and integrate PagerDuty into AI-driven runbooks


## Available Tools
- **create_incident**: Requires the From header email (your PagerDuty user email), service ID, and incident title.

Create a new incident on a service
- **get_incident**: Get detailed information about a specific incident
- **get_service**: Get detailed configuration of a specific service
- **get_user**: Get detailed information about a specific user
- **list_oncalls**: List who is currently on-call across all schedules
- **list_schedules**: List all on-call schedules
- **list_services**: List all monitored services
- **list_users**: List all users in the PagerDuty account
- **update_incident**: Use to acknowledge, resolve, or reassign incidents programatically.

Update an incident status (acknowledge, resolve, escalate)
- **list_escalation_policies**: List all escalation policies
- **list_incidents**: Optionally filter by status: triggered, acknowledged, resolved.

List incidents across all services


## Installation & Usage

To install and use the **PagerDuty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagerduty](https://vinkius.com/mcp/pagerduty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# PagerDuty MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagerduty)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pagerduty-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pagerduty-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage incidents, services, on-call schedules, and escalation policies via PagerDuty — trigger, acknowledge, and resolve alerts from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PagerDuty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all triggered incidents right now."

**🤖 AI Agent:**
> There are 3 triggered incidents:

1. 🔴 **P8K2LMN** — Database connection pool exhausted (Production API)
2. 🔴 **P3J9FGH** — SSL certificate expires in 24h (CDN Edge)
3. 🟡 **P1A4BCD** — High memory usage on worker-03 (Background Jobs)

Would you like me to acknowledge any of these?

---

**👤 You:**
> "Who is on-call for the Platform team right now?"

**🤖 AI Agent:**
> Current on-call for Platform:

- **Level 1**: sarah.chen@company.com (until Apr 7, 9:00 AM UTC)
- **Level 2**: marcus.ops@company.com (until Apr 14, 9:00 AM UTC)

Escalation Policy: Platform Critical (30 min timeout per level).

---

**👤 You:**
> "Acknowledge incident P8K2LMN and show me the service details."

**🤖 AI Agent:**
> ✅ Incident **P8K2LMN** acknowledged successfully.

**Service: Production API**
- Status: Active (Critical)
- Escalation: Platform Critical (3 levels)
- Integrations: Datadog, Sentry, Slack
- Auto-resolve: 4 hours

Would you like me to investigate the root cause or resolve this incident?


## Installation & Usage

To install and use the **PagerDuty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagerduty](https://vinkius.com/mcp/pagerduty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

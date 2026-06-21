# FireHydrant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firehydrant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firehydrant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firehydrant-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Manage incidents, services, and responder teams via AI agents with FireHydrant.

## Description
Connect your **FireHydrant** account to any AI agent and automate your incident management workflows through the Model Context Protocol (MCP). FireHydrant provides a comprehensive platform for declaring incidents, managing service catalogs, and coordinating team responses. Now, you can manage your site reliability and incident response directly through natural conversation.

### What you can do

- **Incident Management** — Declare new incidents, list active ones, and update milestones or fields instantly.
- **Service Catalog** — Access and list all defined services to understand impact and dependencies during an outage.
- **Team Coordination** — List and manage responder teams to ensure the right people are assigned to every incident.
- **Timeline Updates** — Post notes and status updates directly to an incident's timeline from your chat interface.
- **Runbook Execution** — List active runbooks to understand the automated workflows available for your response.
- **Post-Incident Analysis** — Retrieve retrospectives and post-incident reviews to facilitate learning and improvement.
- **Change Tracking** — List change events to identify recent infrastructure or code changes that might have triggered an incident.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FireHydrant API Key (found in your Settings > API Keys)
3. Start managing your incident response from Claude, Cursor, or any MCP client

### Who is this for?

- **SREs & DevOps Engineers** — quickly declare incidents and fetch service details during high-pressure outages.
- **Incident Commanders** — automate the gathering of team information and timeline updates through simple AI commands.
- **Engineering Managers** — get an overview of active incidents and recent change events to keep stakeholders informed.


## Available Tools
- **add_incident_note**: Add note to incident
- **create_incident**: Create a new incident
- **get_incident**: Get incident details
- **get_service**: Get service details
- **get_team**: Get team details
- **list_change_events**: List change events
- **list_incidents**: List incidents
- **list_retrospectives**: List retrospectives
- **list_runbooks**: List active runbooks
- **list_services**: List service catalog
- **list_teams**: List responder teams
- **update_incident**: Update an incident


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FireHydrant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently active incidents in FireHydrant."

**🤖 AI Agent:**
> Checking for active incidents... I found 2 ongoing incidents: 'Database Latency Issue' (sev-2) and 'Payment Gateway Timeout' (sev-1). Would you like the details for any of these?

---

**👤 You:**
> "Declare a new sev-2 incident: 'Redis Connection Spikes'."

**🤖 AI Agent:**
> Incident declared! I've created a new sev-2 incident named 'Redis Connection Spikes'. The incident ID is 'inc_123'. Responder teams are being notified.

---

**👤 You:**
> "Add a note to incident 'inc_123': 'Investigating potential cache invalidation issue'."

**🤖 AI Agent:**
> Note added! Your update has been successfully posted to the timeline for incident 'inc_123'. Responders will see this investigation update immediately.


## Installation & Usage

To install and use the **FireHydrant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firehydrant](https://vinkius.com/mcp/firehydrant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

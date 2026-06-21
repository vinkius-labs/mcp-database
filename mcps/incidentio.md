# Incident.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/incidentio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/incidentio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/incidentio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage incidents, roles, and on-call schedules via Incident.io API.

## Description
Empower your AI agents to manage your incident response lifecycle with Incident.io. This MCP server allows you to list and retrieve incidents, manage roles and types, track custom fields, and view on-call schedules directly through the Incident.io API. Ideal for automating SRE workflows and incident coordination.


## Available Tools
- **get_incident**: Retrieves details for a specific incident
- **list_catalog_types**: Lists all defined catalog types
- **list_custom_fields**: Lists all defined custom fields
- **list_incident_roles**: Lists all defined incident roles
- **list_incident_types**: Lists all defined incident types
- **list_incidents**: Lists all incidents
- **list_schedules**: Lists all on-call schedules
- **list_severities**: Lists all defined incident severities
- **list_teams**: Lists all teams
- **list_users**: Lists all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incident.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ongoing incidents in Incident.io."

**🤖 AI Agent:**
> I'll fetch the list of current incidents for you.

---

**👤 You:**
> "Show me the on-call schedules for this week."

**🤖 AI Agent:**
> I'll retrieve the active on-call schedules from Incident.io.

---

**👤 You:**
> "Check the details for incident ID 'abc-123'."

**🤖 AI Agent:**
> I'll look up the full details and history for that specific incident.


## Installation & Usage

To install and use the **Incident.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incidentio](https://vinkius.com/mcp/incidentio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

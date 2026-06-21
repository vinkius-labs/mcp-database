# Safepoint MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/safepoint)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/safepoint-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/safepoint-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Protect your business data with secure backup, disaster recovery, and cloud-to-cloud replication for critical SaaS applications.

## Description
Connect your **Safepoint** account to any AI agent and take full control of your lone worker safety orchestration and team monitoring through natural conversation. Safepoint provides a premier platform for protecting workers in high-risk or isolated environments, and this integration allows you to retrieve user metadata, monitor real-time safety alerts, and manage daily tasks directly from your chat interface.

### What you can do

- **Safety Alert & Emergency Orchestration** — Monitor real-time safety alerts and retrieve detailed incident metadata to ensure rapid response directly from the AI interface.
- **User & Team Lifecycle Management** — List all managed users and retrieve detailed profile metadata, including team assignments programmatically.
- **Task & Activity Intelligence** — Create and monitor safety tasks and retrieve live location metadata via natural language to keep your mobile workforce protected.
- **Historical Safety Oversight** — Access historical activity and event logs to maintain comprehensive compliance records and audit trails.
- **Operational Monitoring** — Track system activity and manage organizational safety metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Safepoint API Token from your web portal settings
3. Start managing your team safety from Claude, Cursor, or any MCP-compatible client

No more manual check-ins or siloed safety logs. Your AI acts as a dedicated safety coordinator or operations supervisor.

### Who is this for?

- **Health & Safety Officers** — quickly retrieve incident details and monitor worker statuses without switching apps.
- **Operations Managers** — automate the creation of daily safety tasks and track team locations via natural conversation.
- **Team Leads** — streamline the retrieval of user metadata and monitor real-time safety compliance directly within the chat.


## Available Tools
- **create_safety_task**: Create a new lone worker task
- **get_alert_details**: Get details for a specific alert
- **get_location**: Get details for a specific location
- **get_safepoint_user_details**: Get user details
- **list_safety_alerts**: List recent safety alerts
- **list_safety_events**: List recent safety events
- **list_safety_history**: List historical safety data
- **list_user_locations**: List current user locations
- **list_safety_tasks**: List all active safety tasks
- **list_safepoint_teams**: List all safety teams
- **list_safepoint_users**: List all users in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Safepoint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active safety alerts in Safepoint."

**🤖 AI Agent:**
> I've retrieved your alerts. You have 2 active incidents: 'SOS Alert' (User: John) and 'Fall Detected' (User: Sarah). Would you like the precise location for any of them?

---

**👤 You:**
> "Show me all active safety alerts and their severity levels across all monitored locations."

**🤖 AI Agent:**
> 7 active safety alerts. Critical (2): "Fire alarm triggered" at Building A, Floor 3 (10:23 AM, emergency services notified), "Unauthorized access attempt" at Server Room B (10:45 AM, security team dispatched). High (2): "Environmental sensor warning" at Warehouse 2 (temperature 42°C), "Equipment malfunction" at Production Line 3. Medium (2): "Access badge expired" for 12 employees, "CCTV offline" at Parking Lot C. Low (1): "Scheduled maintenance reminder" for Building B HVAC. All locations monitored: 14.

---

**👤 You:**
> "Create a new safety task for the maintenance team to inspect all emergency exits in Building A."

**🤖 AI Agent:**
> Safety task created: "Emergency Exit Inspection - Building A". Assigned to: Maintenance Team (5 members). Location: Building A (8 emergency exits across 4 floors). Checklist: door functionality, signage visibility, pathway clearance, alarm testing, lighting verification. Due date: May 20, 2025. Priority: High (post-fire alarm incident). Compliance requirement: OSHA 1910.37. Previous inspection: March 15, 2025 (all passed). Photo documentation required for each exit.


## Installation & Usage

To install and use the **Safepoint** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safepoint](https://vinkius.com/mcp/safepoint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

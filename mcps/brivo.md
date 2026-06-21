# Brivo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brivo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brivo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brivo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage your access control via Brivo — unlock doors, track access events, and oversee users directly from any AI agent.

## Description
Connect your **Brivo Access** account to any AI agent and orchestrate your physical security, facility management, and user provisioning workflows through natural conversation.

### What you can do

- **Door Control & Status** — List all access points, check their live status (open/closed/locked), and trigger momentary unlocks directly from your workspace.
- **User Provisioning** — List and retrieve detailed profiles for all users and manage their access groups and credentials.
- **Event Monitoring** — Retrieve real-time or historical access events and security alarms to ensure facility safety.
- **Credential Oversight** — List and audit physical and digital credentials (cards, mobile passes) assigned to users.
- **Schedule Coordination** — Access time schedules used for automated locking and unlocking of your facility.

### How it works

1. Subscribe to this server
2. Enter your Brivo API Key, Username, and Password
3. Start managing your facility security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security & Facility Managers** — quickly unlock doors for visitors or check facility status without manual portal logins.
- **IT Admins** — retrieve user access profiles and credential statuses straight from their workflow tools.
- **Ops Leads** — monitor security events and team access using natural language.


## Available Tools
- **get_account_info**: Retrieve core account/site information
- **get_door_status**: Get live status of a door
- **get_user**: Get details of a specific user
- **list_doors**: List all access points (doors)
- **list_credentials**: List all access credentials (cards, pass, etc)
- **list_access_events**: List recent access events and alarms
- **list_access_groups**: List all access groups
- **list_schedules**: List time schedules for access
- **list_users**: List all people/users in the system
- **unlock_door**: Momentarily unlock a door


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the doors in my office."

**🤖 AI Agent:**
> I've retrieved your access points. You have 4 doors: 'Main Entrance' (ID: 101), 'Server Room' (ID: 102), 'Back Exit' (ID: 103), and 'HR Suite' (ID: 104).

---

**👤 You:**
> "Unlock the 'Main Entrance' door (ID 101)."

**🤖 AI Agent:**
> Unlocking 'Main Entrance'... Success! The door is now unlocked for the configured momentary period.

---

**👤 You:**
> "Show the recent access events for the Server Room."

**🤖 AI Agent:**
> Retrieving events... John Doe accessed the Server Room at 9:15 AM today, and Alice Smith accessed it at 10:30 AM. There are no active alarms.


## Installation & Usage

To install and use the **Brivo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brivo](https://vinkius.com/mcp/brivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

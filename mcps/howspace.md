# Howspace MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/howspace)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/howspace-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/howspace-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Facilitate collaborative learning and organizational development with AI-powered workshops that engage participants at scale.

## Description
Connect your **Howspace** account to any AI agent and manage your collaborative workspaces through natural conversation.

### What you can do

- **Workspace Management** — List all workspaces, create new ones, and inspect individual workspace details and settings
- **Participant Management** — Browse participants in any workspace and add new members by email with optional name fields
- **Campaign Management** — List all campaigns configured for engagement and communication
- **Profile Access** — Retrieve information about the authenticated API user

### How it works

1. Subscribe to this server
2. Enter your Howspace Base URL and API Key
3. Start managing workspaces from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Facilitators** — create workspaces, add participants, and manage collaborative sessions without opening the dashboard
- **HR & L&D Teams** — onboard new employees into training workspaces and track campaign engagement
- **Change Management Consultants** — manage large-scale workshops and stakeholder engagement through AI


## Available Tools
- **add_participant**: Add a participant to a workspace
- **create_workspace**: Create a new workspace
- **get_me**: Get current user info
- **get_workspace**: Get details of a specific workspace
- **list_campaigns**: List all campaigns
- **list_participants**: List participants in a workspace
- **list_workspaces**: List all workspaces in Howspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Howspace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new workspace called 'Q3 Strategy Workshop' and add 3 team members."

**🤖 AI Agent:**
> Workspace created! Name: 'Q3 Strategy Workshop', ID: ws_4521. Adding participants: 1) sarah@company.com (Sarah Chen) — ✅ Added. 2) mike@company.com (Mike Torres) — ✅ Added. 3) lisa@company.com (Lisa Park) — ✅ Added. All 3 participants will receive email invitations. The workspace is now ready for content configuration. You have 12 total workspaces in your account. Would you like to list all workspaces or check the campaigns?

---

**👤 You:**
> "Show all workspaces and the participants in the onboarding workspace."

**🤖 AI Agent:**
> Your workspaces: 12 total. 1) 'Employee Onboarding 2025' (ws_4001, 45 participants). 2) 'Leadership Development' (ws_4002, 28 participants). 3) 'Q3 Strategy Workshop' (ws_4521, 3 participants). 4-12) 9 other workspaces. Participants in 'Employee Onboarding 2025' (45 total): Recent additions: 1) Ana Müller (ana@company.com, added Apr 22). 2) James Rodriguez (james@company.com, Apr 20). 3) Chen Wei (wei@company.com, Apr 18). Facilitators: Sarah Chen, Mike Torres. Would you like to add more participants or view campaigns?

---

**👤 You:**
> "List all campaigns and show my account details."

**🤖 AI Agent:**
> Your profile: Sarah Chen (sarah@company.com), Role: Admin, Organization: Acme Corp. Active campaigns: 4. 1) 'New Hire Welcome' — triggers on participant addition to 'Employee Onboarding 2025', sends welcome email + first assignment. 2) 'Weekly Engagement Pulse' — runs every Monday, surveys all active workspace participants. 3) 'Leadership Reflection' — biweekly prompt in 'Leadership Development' workspace. 4) 'Workshop Reminder' — 24h before scheduled sessions. Total campaign reach: 145 participants across all workspaces. Would you like to create a new workspace or add participants?


## Installation & Usage

To install and use the **Howspace** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/howspace](https://vinkius.com/mcp/howspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

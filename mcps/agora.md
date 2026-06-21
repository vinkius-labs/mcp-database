# Agora MCP Server

Orchestrate Agora real-time engagement — manage channels, monitor usage, and handle cloud recording directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/agora)

## Overview
**Category:** infrastructure
**Tools Count:** 10

## Description
Connect your AI agents to **Agora**, the leading real-time engagement platform for video, voice, and interactive streaming. This MCP provides 10 tools to manage communication channels, orchestrate cloud recording sessions, and monitor granular usage metrics programmatically.

### What you can do

- **Channel Orchestration** — Create and manage RTC (Real-Time Communication) channels and list active users within each session
- **Cloud Recording** — Start, stop, and query the status of cloud recording tasks for archival or auditing purposes
- **Usage Monitoring** — Retrieve detailed metrics on minutes consumed, bandwidth, and concurrent user peaks
- **Project Insights** — List and inspect project configurations, including AppIDs and token settings, directly from your agent
- **Rule Management** — Configure channel-level rules and settings to optimize the interactive experience

### How it works

1. Subscribe to this server
2. Log in to the [**Agora Console**](https://console.agora.io/)
3. Navigate to **Project Management** and select your active project
4. Obtain your **Customer ID**, **Customer Secret**, and **AppID** from the console settings
5. Insert your credentials into the fields below to start managing your real-time engagement workflows.

### Who is this for?

- **Full-Stack Developers** — automate the provisioning of communication channels and recording sessions
- **Live Ops Teams** — monitor real-time usage peaks and system health across multiple Agora projects
- **Product Managers** — retrieve monthly consumption reports and user engagement data via natural language


## Available Tools
- **acquire_cloud_recording**: Required before starting.

Request a resource ID for cloud recording
- **create_project**: Create a new Agora project
- **get_project_details**: Get detailed information for a specific project
- **get_usage_stats**: Query usage data for a specific project
- **list_active_calls**: List ongoing calls and sessions
- **list_projects**: List all Agora projects in your console
- **list_whiteboard_rooms**: List active Interactive Whiteboard rooms
- **query_cloud_recording**: Check the status of an active recording
- **start_cloud_recording**: Start recording a channel to the cloud
- **stop_cloud_recording**: Stop an ongoing cloud recording


## Installation & Usage

To install and use the **Agora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agora](https://vinkius.com/mcp/agora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Agora MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agora)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/agora-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/agora-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Orchestrate Agora real-time engagement — manage channels, monitor usage, and handle cloud recording directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users currently connected to Agora channel 'room_101' in project 'app_abc'."

**🤖 AI Agent:**
> Retrieving channel users... I found 3 UIDs connected to 'room_101': 1. UID: 777, 2. UID: 888, 3. UID: 999. Would you like to check the connection quality for any of these users?

---

**👤 You:**
> "Start a cloud recording for channel 'webinar_live' with AppID 'my_agora_app_id'."

**🤖 AI Agent:**
> Initializing Agora cloud recording... Success! The recording session for 'webinar_live' has started. Resource ID: `res_xyz123`, SID: `sid_789abc`. I will monitor the status for you.

---

**👤 You:**
> "Show my project's RTC usage for the last 7 days."

**🤖 AI Agent:**
> Fetching Agora usage metrics... In the last 7 days, your project consumed 1,200 video minutes (HD) and 450 audio minutes. Peak concurrency was 25 users on April 10th.


## Installation & Usage

To install and use the **Agora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agora](https://vinkius.com/mcp/agora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

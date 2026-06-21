# Dotcom-Monitor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dotcom-monitor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dotcom-monitor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dotcom-monitor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor website uptime, page load speed, and server health from multiple global locations with instant alert notifications.

## Description
Connect your **Dotcom-Monitor** monitoring account to any AI agent and simplify how you oversee your website uptime, server performance, and global monitoring locations through natural conversation.

### What you can do

- **Device Oversight** — List all configured monitoring devices (uptime, speed, API) and retrieve detailed configuration metadata.
- **Performance Tracking** — Query historical status data and response times to identify latency trends via AI.
- **Global Monitoring** — List available geographic locations and verify where your checks are running from.
- **Alert Management** — Query configured alert groups and notification teams to ensure your incident response is ready.
- **Platform Analysis** — List available monitoring platforms (ServerView, UserView, WebAPI) to coordinate your checks.
- **Operational Monitoring** — Check real-time device health and verify system connectivity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Dotcom-Monitor API Key (found in your account settings)
3. Start monitoring your digital assets from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & SREs** — quickly retrieve historical performance logs and verify device statuses via simple AI commands.
- **IT Managers** — monitor global uptime and verify alert group configurations directly from the workspace.
- **Web Developers** — check response times and verify platform availability via the AI assistant.


## Available Tools
- **get_device_details**: Get details for a specific device
- **get_device_monitoring_history**: Get historical status for a device
- **list_alert_groups**: List configured alert groups
- **list_monitoring_devices**: List monitoring devices
- **list_monitoring_locations**: List geographic monitoring locations
- **list_available_platforms**: ).

List monitoring platforms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dotcom-Monitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active monitoring devices in my account."

**🤖 AI Agent:**
> I've retrieved your monitoring devices. You have 5 active monitors including 'Homepage Uptime', 'API Gateway Check', and 'Checkout Flow'. Which one would you like to see detailed status for?

---

**👤 You:**
> "Show me the monitoring history for device 'dev_10293'."

**🤖 AI Agent:**
> Fetching history... For device dev_10293, the uptime over the last 24 hours was 100%. Average response time was 120ms, with a peak of 450ms at 3 AM. Would you like to see the error logs?

---

**👤 You:**
> "What are the available alert groups in my account?"

**🤖 AI Agent:**
> Retrieving alert groups... You have 3 groups configured: 'Core Infrastructure' (Email/SMS), 'Frontend Devs' (Slack), and 'Stakeholders' (Weekly Email Report). Shall I verify the members for any of these?


## Installation & Usage

To install and use the **Dotcom-Monitor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dotcom-monitor](https://vinkius.com/mcp/dotcom-monitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

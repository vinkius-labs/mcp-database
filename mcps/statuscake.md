# StatusCake MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/statuscake)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/statuscake-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/statuscake-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor website uptime, page speed, and SSL certificates directly from your AI agent using StatusCake.

## Description
Connect your **StatusCake** account to any AI agent to monitor your infrastructure's health and performance through natural conversation.

### What you can do

- **Uptime Monitoring** — List, create, and manage uptime tests to ensure your services are always reachable and performing correctly.
- **Page Speed Analysis** — Track loading times and performance metrics across different global regions to optimize user experience.
- **SSL Certificate Tracking** — Monitor certificate expiration dates and security configurations to avoid unexpected downtime or security warnings.
- **Heartbeat Checks** — Manage cron job and background task monitoring to ensure your internal processes and backups are running as scheduled.
- **Alerting & Maintenance** — View contact groups and maintenance windows to understand your notification flow and planned outages.

### How it works

1. Subscribe to this server
2. Enter your StatusCake API Key
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

No more manually checking dashboards to see if your site is down. Your AI acts as a 24/7 SRE or DevOps assistant.

### Who is this for?

- **DevOps Engineers** — quickly check the status of all monitors and manage maintenance windows without leaving the terminal or editor.
- **SRE Teams** — automate the retrieval of uptime reports and heartbeat statuses during incident response.
- **Web Developers** — monitor page speed metrics and SSL health directly from the coding environment.


## Available Tools
- **create_heartbeat**: Create a heartbeat check
- **create_pagespeed**: Create a pagespeed check
- **create_ssl_check**: Create an SSL check
- **create_uptime**: Create an uptime check
- **delete_heartbeat**: Delete a heartbeat check
- **delete_pagespeed**: Delete a pagespeed check
- **delete_ssl_check**: Delete an SSL check
- **delete_uptime**: Delete an uptime check
- **get_heartbeat**: Retrieve a heartbeat check
- **get_pagespeed_history**: Get pagespeed check history
- **get_pagespeed**: Retrieve a pagespeed check
- **get_ssl_check**: Retrieve an SSL check
- **get_uptime**: Retrieve an uptime check
- **list_contact_groups**: Get all contact groups
- **list_heartbeat_locations**: Get Heartbeat Locations
- **list_heartbeats**: Get all heartbeat checks
- **list_maintenance_windows**: Get all maintenance windows
- **list_pagespeed_locations**: Get Page Speed Locations
- **list_pagespeeds**: Get all pagespeed checks
- **list_ssl_locations**: Get SSL Locations
- **list_ssl_checks**: Get all SSL checks
- **list_uptime_locations**: Get Uptime Locations
- **list_uptimes**: Get all uptime checks
- **update_heartbeat**: Update a heartbeat check
- **update_pagespeed**: Update a pagespeed check
- **update_ssl_check**: Update an SSL check
- **update_uptime**: Update an uptime check


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StatusCake** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active uptime monitors."

**🤖 AI Agent:**
> I've retrieved your uptime monitors. You have 3 active tests: 'Main API' (ID: 101), 'Customer Portal' (ID: 102), and 'Legacy DB' (ID: 103). All are currently reporting 'Up'.

---

**👤 You:**
> "Create a new heartbeat check named 'Daily Backup' with a period of 86400 seconds."

**🤖 AI Agent:**
> Successfully created the heartbeat check 'Daily Backup'. The system will now expect a signal every 24 hours. The Test ID is 55012.

---

**👤 You:**
> "Show me the details for SSL monitor ID 998877."

**🤖 AI Agent:**
> Inspecting SSL monitor 998877... The certificate for 'secure.example.com' is valid. It expires in 45 days (2024-12-15) and is issued by Let's Encrypt.


## Installation & Usage

To install and use the **StatusCake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/statuscake](https://vinkius.com/mcp/statuscake)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

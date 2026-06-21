# Baota Panel / 宝塔面板 API MCP Server

Leading server management panel in China — manage websites, databases, and system resources via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/baota-panel-api)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Empower your AI agent to orchestrate your server infrastructure with **Baota Panel** (宝塔面板), the dominant web hosting control panel in China. By connecting Baota to your agent, you transform complex server administration, website maintenance, and resource monitoring into a natural conversation. Your agent can instantly list managed websites, retrieve real-time system load, monitor database health, and even browse administrative logs without you ever needing to log in to the panel interface. Whether you are conducting a security audit or monitoring server performance, your agent acts as a real-time SRE assistant, keeping your infrastructure accurate and your services online.

### What you can do

- **Site Orchestration** — List and retrieve detailed information about all websites managed by your Baota Panel.
- **Resource Monitoring** — Get real-time system load, CPU usage, and RAM statistics to audit server health.
- **Database Management** — List all databases and retrieve metadata for your data storage infrastructure.
- **Operational Auditing** — Browse cron jobs, pending background tasks, and recent administrative logs.
- **Software Insights** — List installed software and plugins (Nginx, PHP, MySQL) to ensure your stack is up-to-date.

### How it works

1. Subscribe to this server
2. Enter your Panel Host, API Secret Key, and API ID
3. Ensure your caller IP is whitelisted in the Baota Panel settings
4. Start managing your server through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Server Administrators** — monitor system resources and coordinate maintenance through natural language queries.
- **Web Developers** — manage site configurations and audit database lists directly from your AI-powered workspace.
- **DevOps Engineers** — oversee cron tasks and monitor network traffic via a unified AI interface.
- **Baota Power Users** — integrate your existing server workflows into your AI-driven daily routines.


## Available Tools
- **get_disk_info**: Get disk usage
- **get_network_info**: Get network status
- **get_software_list**: ).

List installed software
- **get_system_total**: Get system load info
- **get_task_count**: Get pending task count
- **list_cron_tasks**: List cron jobs
- **list_databases**: List databases
- **list_ftp**: List FTP accounts
- **list_logs**: List panel logs
- **list_sites**: List websites


## Installation & Usage

To install and use the **Baota Panel / 宝塔面板 API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baota-panel-api](https://vinkius.com/mcp/baota-panel-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

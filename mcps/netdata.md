# Netdata MCP Server

Monitor real-time infrastructure metrics, analyze system performance, and track active alerts across your nodes and Netdata Cloud spaces.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/netdata)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

## Description
Connect your **Netdata** monitoring infrastructure to any AI agent for instant, real-time observability and performance analysis through natural language.

### What you can do

- **Real-time Metrics** — Fetch granular data from specific charts (CPU, RAM, Disk, Network) using `get_chart_data` to diagnose performance bottlenecks.
- **Agent Health** — Inspect node versions, host information, and enabled features with `get_agent_info` and `list_charts`.
- **Alert Management** — Query active alarms on local agents via `get_alarms` or monitor space-wide critical issues using `list_space_alerts`.
- **Cloud Orchestration** — Navigate your entire infrastructure by listing spaces, rooms, and nodes connected to Netdata Cloud.
- **Scraping & Export** — Retrieve all metrics in a format suitable for external analysis tools using `get_all_metrics`.

### How it works

1. Subscribe to this server
2. Enter your Netdata Cloud Token or Agent URL
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

No more jumping between dashboards to find which node is spiking. Your AI acts as a 24/7 SRE or System Administrator.

### Who is this for?

- **DevOps Engineers** — instantly correlate system alerts with recent deployments without leaving the terminal or IDE.
- **SREs** — automate the retrieval of chart data and alarm statuses to speed up incident response.
- **System Administrators** — manage large-scale node environments by querying spaces and rooms via simple conversation.


## Available Tools
- **get_alarms**: Get current status of all configured alarms
- **get_all_metrics**: Get all metrics for scraping
- **list_charts**: ).

List all available charts on the node
- **get_chart_data**: Fetch metric data from a specific chart
- **get_agent_info**: Get Netdata Agent information
- **list_room_nodes**: List nodes within a specific room
- **list_rooms**: List rooms within a specific space
- **list_space_alerts**: Fetch active alerts across the space
- **list_space_nodes**: List all nodes connected to a space
- **list_spaces**: List all Netdata Cloud spaces


## Installation & Usage

To install and use the **Netdata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netdata](https://vinkius.com/mcp/netdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

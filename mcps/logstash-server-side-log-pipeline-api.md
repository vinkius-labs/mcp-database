# Logstash (Server-side Log Pipeline API) MCP Server

Monitor and manage Logstash instances — check node health, inspect pipeline statistics, and troubleshoot hot threads directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/logstash-server-side-log-pipeline-api)

## Overview
**Category:** devops-cicd
**Tools Count:** 6

## Description
Connect your **Logstash** instance to any AI agent to monitor and manage your server-side data processing pipelines through natural conversation.

### What you can do

- **Health Monitoring** — Get instant reports on the health status of your Logstash nodes and pipelines (Green/Yellow/Red).
- **Performance Metrics** — Retrieve detailed JVM, process, and event flow statistics to identify bottlenecks.
- **Node Inspection** — Access configuration details, OS environment, and pipeline settings.
- **Troubleshooting** — Identify performance issues by fetching current hot threads in real-time.
- **Plugin Management** — List all installed plugins and their versions to ensure environment consistency.

### How it works

1. Subscribe to this server
2. Enter your Logstash API URL and credentials (if applicable)
3. Start monitoring your data pipelines from Claude, Cursor, or any MCP-compatible client

No more manual curl commands to port 9600. Your AI acts as a dedicated systems administrator or SRE.

### Who is this for?

- **DevOps Engineers** — instantly check node health and JVM metrics without leaving the terminal or chat interface
- **SRE Teams** — troubleshoot performance bottlenecks by inspecting hot threads during incidents
- **Data Engineers** — verify pipeline settings and plugin versions across different environments


## Available Tools
- **get_health_report**: Get Logstash health report
- **get_hot_threads**: Useful for troubleshooting performance issues.

Get Logstash hot threads
- **get_node_info**: Get Logstash node information
- **get_plugins_info**: Get Logstash plugins information
- **get_root**: Get Logstash root information
- **get_node_stats**: Get Logstash node statistics


## Installation & Usage

To install and use the **Logstash (Server-side Log Pipeline API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logstash-server-side-log-pipeline-api](https://vinkius.com/mcp/logstash-server-side-log-pipeline-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

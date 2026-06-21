# Tencent START MCP Server

Orchestrate Tencent START Cloud Gaming (GS) — manage server sessions, monitor workers, and scale capacity directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-start)

## Overview
**Category:** industry-titans
**Tools Count:** 11

## Description
Connect your AI agents to **Tencent START Cloud Gaming (GS)**, the high-performance PaaS platform for cloud-native gaming. This MCP provides 11 tools to automate game instance locking, session creation, and scaling management.

### What you can do

- **Session Lifecycle** — Lock workers, create server sessions, and stop games programmatically
- **Resource Management** — Monitor worker status and availability across different game IDs
- **User Monitoring** — Track concurrent users and worker assignments in real-time
- **Capacity Scaling** — Modify concurrency limits to dynamically adjust to player demand

### How it works

1. Subscribe to this server
2. Log in to the [**Tencent Cloud Console**](https://console.cloud.tencent.com/gs)
3. Navigate to **Access Management (CAM)** and generate a **SecretId** and **SecretKey**
4. Enable the **Cloud Gaming (GS)** service
5. Copy your credentials and preferred **Region** into the fields below

### Who is this for?

- **Game Developers** — automate backend orchestration for cloud-native titles
- **Platform Operators** — monitor resource utilization and concurrent user metrics
- **Infrastructure Engineers** — scale cloud gaming capacity based on real-time demand


## Available Tools
- **create_session**: Initialize a cloud gaming session
- **get_capacity_limit**: Check max concurrent user limit for a game
- **get_concurrent_user_info**: Check current concurrency for a game
- **get_worker_info**: Get worker info for a specific user
- **list_games**: List games available on the Tencent GS platform
- **list_workers**: List status of cloud gaming workers
- **modify_capacity_limit**: Update max concurrent user limit for a game
- **stop_game**: Ends a game session and releases the instance
- **stop_publish_stream_by_action**: Stops the video stream using an explicit action code
- **stop_publish_stream**: Stops the video stream for a specific user
- **try_lock_worker**: Locks a cloud gaming instance for a specific user


## Installation & Usage

To install and use the **Tencent START** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-start](https://vinkius.com/mcp/tencent-start)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

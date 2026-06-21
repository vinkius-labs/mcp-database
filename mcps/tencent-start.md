# Tencent START MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-start)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Tencent START Cloud Gaming (GS) — manage server sessions, monitor workers, and scale capacity directly from any AI agent.

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


## Available Tools (11)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent START** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all cloud games available in region 'ap-guangzhou'."

**🤖 AI Agent:**
> I've fetched the game catalog for 'ap-guangzhou'. You have 3 active titles: 'League of Legends' (ID: game_101), 'CrossFire' (ID: game_202), and 'Naraka' (ID: game_303). Would you like to check the worker status for any of these?

---

**👤 You:**
> "Check the status of workers for game 'game_101'."

**🤖 AI Agent:**
> Querying worker status for 'League of Legends'... I found 50 total workers: 35 are 'Occupied', 12 are 'Idle' (Ready), and 3 are in 'Maintenance'.

---

**👤 You:**
> "Modify the concurrency limit for game 'game_202' to 100 users."

**🤖 AI Agent:**
> Connecting to capacity management... Concurrency limit for 'CrossFire' (ID: game_202) has been successfully updated to 100. The infrastructure is scaling to match.


## ❓ FAQ

**Q: Can I automatically list all available games on the platform?**
Yes! Use the `list_games` tool. It will retrieve metadata for all configured cloud games, including their names and unique identifiers.

**Q: How do I check the status of my cloud gaming workers?**
Use the `list_workers` tool. It returns the availability and current operational state of all server instances allocated to your account.

**Q: Can I dynamically modify the concurrency limit for a game?**
Yes! Use the `modify_capacity_limit` tool with the target Game ID and the new maximum concurrent user count to scale your capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-start](https://vinkius.com/mcp/tencent-start)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tencent START** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tencent-start` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tencent START** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tencent-start": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

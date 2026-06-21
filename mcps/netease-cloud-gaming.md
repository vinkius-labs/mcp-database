# NetEase Cloud Gaming MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netease-cloud-gaming)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/netease-cloud-gaming-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/netease-cloud-gaming-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage NetEase Cloud Gaming sessions — orchestrate server instances, monitor user quotas, and scaling capacity directly from any AI agent.

## Description
Connect your AI agents to **NetEase Cloud Gaming (网易云游戏)**, the leading platform for instant cloud-native gaming. This MCP provides 10 tools to manage the entire lifecycle of cloud gaming sessions and user access controls.

### What you can do

- **Session Control** — Create, stop, and monitor cloud gaming sessions with real-time status updates
- **Catalog Management** — List optimized games and retrieve detailed technical specifications
- **Quota Orchestration** — Monitor and adjust user play time quotas and subscription limits
- **Infrastructure Monitoring** — Inspect server clusters and check global system health

### How it works

1. Subscribe to this server
2. Register at the [**NetEase Games Developer Platform**](https://open.163.com/)
3. Apply for the **Cloud Gaming (大神云)** service access
4. Generate your **AccessKey** and **SecretKey** from the developer console
5. Configure your integration in Vurb to start managing your cloud gaming instances.

### Who is this for?

- **Game Developers** — bridge in-game events with cloud instance lifecycle management
- **Live Operations** — monitor server health and user session distribution
- **Platform Integrators** — build custom cloud gaming portals using NetEase infrastructure


## Available Tools
- **add_user_quota**: Add cloud play time to a user account
- **create_session**: Initialize a new NetEase cloud gaming session
- **get_cluster_info**: Get detailed info for a specific cluster
- **get_game_detail**: Get details for a specific NetEase cloud game
- **get_session_status**: Check the status of a cloud gaming session
- **get_system_health**: Check overall health of the NetEase Cloud Gaming platform
- **get_user_quota**: Get remaining cloud play time for a user
- **list_clusters**: List cloud gaming server clusters
- **list_games**: List games available on NetEase Cloud Gaming
- **stop_session**: Force stop an active cloud gaming session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NetEase Cloud Gaming** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a cloud gaming session for game 'game_456' and user 'user_789'."

**🤖 AI Agent:**
> Initializing NetEase cloud instance... Session created successfully. ID: `sess_abc123`. The game is now loading on the remote server. Would you like to monitor the session status?

---

**👤 You:**
> "List all games currently available on the NetEase Cloud platform."

**🤖 AI Agent:**
> Retrieving NetEase game catalog... I found several optimized titles including: 1. Onmyoji (ID: g1), 2. Naraka: Bladepoint (ID: g2), 3. Identity V (ID: g3). Which one would you like to launch?

---

**👤 You:**
> "Show the remaining quota for user 'user_beta_1'."

**🤖 AI Agent:**
> Checking user quota... User 'user_beta_1' has 120 minutes of cloud play time remaining out of a total monthly allowance of 500 minutes.


## Installation & Usage

To install and use the **NetEase Cloud Gaming** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netease-cloud-gaming](https://vinkius.com/mcp/netease-cloud-gaming)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

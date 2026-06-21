# 4YouSee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/4yousee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/4yousee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/4yousee-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Digital signage management platform — monitor players, manage media, and audit content via AI.

## Description
Empower your AI agent to orchestrate your entire digital signage network with **4YouSee**, the leading platform for enterprise-grade content delivery. By connecting 4YouSee to your agent, you transform complex network monitoring into a natural conversation. Your agent can instantly audit player connectivity, navigate your media library, and retrieve dynamic templates without you ever touching a dashboard. Whether you are managing thousands of screens or a single retail display, your agent acts as a real-time operations manager, ensuring your signage is always live and impactful.

### What you can do

- **Player Monitoring** — List all players in your network, check their real-time online status, and view technical health details.
- **Media Management** — Browse your entire media library, list available files, and audit content types for consistency.
- **Template Access** — View and manage news templates, dynamic content layouts, and layout metadata.
- **User Auditing** — List authorized platform users and groups to maintain strict organizational control.
- **Network Health** — Quickly identify disconnected players or content delivery bottlenecks directly from chat.

### How it works

1. Subscribe to this server
2. Enter your 4YouSee Manager Secret Token
3. Start managing your digital signage network through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Signage Operators** — monitor large networks of screens and identify technical issues instantly through AI.
- **Marketing Managers** — verify if new campaign media and templates have been correctly uploaded and distributed.
- **IT Support Teams** — perform rapid health checks on player connectivity without manual dashboard logins.
- **Content Curators** — manage news feeds and dynamic signage templates for retail or corporate environments.


## Available Tools
- **list_players**: List all digital signage players
- **get_player**: Get detailed monitoring data for a specific player
- **list_medias**: List all available media files
- **list_templates**: List content and news templates
- **list_users**: List platform users and groups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **4YouSee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all offline players in my 4YouSee network."

**🤖 AI Agent:**
> I've scanned your network and identified 3 offline players. Here are their names and locations so you can take action.

---

**👤 You:**
> "List all uploaded video files in my 4YouSee media library."

**🤖 AI Agent:**
> I've retrieved your media library. You have 12 video files currently available, including 'promo_winter.mp4' and 'brand_loop.mov'. Would you like the full IDs for any of them?

---

**👤 You:**
> "Which dynamic templates are available for my signage network?"

**🤖 AI Agent:**
> I've found 5 active templates in your 4YouSee Manager, including news layouts and weather widgets. I can provide the names and configuration details for each.


## Installation & Usage

To install and use the **4YouSee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/4yousee](https://vinkius.com/mcp/4yousee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

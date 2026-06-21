# iQiyi Open Platform / 爱奇艺开放平台 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iqiyi-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iqiyi-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iqiyi-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading video platform — retrieve user info, VIP status, and search content via AI.

## Description
Empower your AI agent to orchestrate your video entertainment and membership insights with **iQiyi Open Platform** (爱奇艺), the 'Netflix of China'. By connecting iQiyi to your agent, you transform complex user profile retrieval, VIP status auditing, and content discovery into a natural conversation. Your agent can instantly retrieve nickname and avatar data, verify membership levels and expiration dates, search through a massive library of movies and shows, and audit order histories without you ever needing to navigate the comprehensive iQiyi Developer Portal. Whether you are conducting market research on popular rankings or coordinating user engagement, your agent acts as a real-time entertainment coordinator, providing accurate results from a single, authorized source.

### What you can do

- **User Orchestration** — Retrieve basic profile metadata including nicknames and unique identifiers.
- **Membership Auditing** — Verify real-time VIP status, levels, and subscription deadlines for users.
- **Content Discovery** — Search the iQiyi library for movies and shows, and explore popular rankings.
- **Order Management** — List and retrieve detailed metadata for user orders and membership packages.
- **Operational Monitoring** — Verify API connectivity and gateway status to ensure service reliability.

### How it works

1. Subscribe to this server
2. Enter your iQiyi AppKey and MD5 Key
3. Start managing your video data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Entertainment Analysts** — automate routine content searches and popularity reporting through natural language.
- **Platform Managers** — audit user membership status and verify order health directly from your workspace.
- **Developers** — integrate professional-grade video metadata into your AI-driven daily routines.
- **iQiyi Power Users** — integrate your existing project integrations into your AI-driven daily routines.


## Available Tools
- **get_content_metadata**: Get video metadata
- **get_order_info**: Get order details
- **get_user_profile**: Get user information
- **get_video_rankings**: g., hot, new).

Get popular rankings
- **get_vip_status**: Check VIP membership status
- **list_user_orders**: List user orders
- **list_video_categories**: List content categories
- **search_video_content**: Search for movies/shows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iQiyi Open Platform / 爱奇艺开放平台** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'The Wandering Earth' in the iQiyi library."

**🤖 AI Agent:**
> I've searched the iQiyi library for you. I found 'The Wandering Earth' (2019) and several related titles. Would you like me to retrieve the detailed metadata or the latest popularity ranking for this movie?

---

**👤 You:**
> "Check the VIP membership status for token 'SESSION_8821'."

**🤖 AI Agent:**
> I've retrieved the VIP status for the user. They are currently a 'Gold VIP' (Level 5) with an active subscription valid until 2024-12-31. Should I also check their recent order history?

---

**👤 You:**
> "List all available iQiyi membership packages."

**🤖 AI Agent:**
> I've retrieved the membership package list. You have several options including 'Standard Monthly VIP' (25 CNY), 'Quarterly Gold' (68 CNY), and 'Annual Diamond' (248 CNY). Would you like to see the specific benefits for each level?


## Installation & Usage

To install and use the **iQiyi Open Platform / 爱奇艺开放平台** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iqiyi-open-platform](https://vinkius.com/mcp/iqiyi-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

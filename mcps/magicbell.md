# MagicBell MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magicbell)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/magicbell-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/magicbell-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage notifications and broadcasts via MagicBell — list, retrieve, and trigger multi-channel alerts directly from your AI agent.

## Description
Connect your **MagicBell** project to any AI agent to orchestrate multi-channel notification workflows. Trigger broadcasts, check delivery status, and manage communication logs through natural conversation.

### What you can do

- **Broadcast Management** — List all active and past broadcasts sent through your project to track communication history.
- **Detailed Inspection** — Fetch specific broadcast metadata, content, and processing status using unique UUIDs.
- **Trigger Notifications** — Create and send new broadcasts with custom titles, body content, and specific recipient filters.
- **Multi-channel Control** — Handle channel-specific overrides for email, SMS, and push notifications to ensure the right message reaches the right place.

### How it works

1. Subscribe to this server
2. Enter your MagicBell Project JWT
3. Start sending and monitoring notifications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — trigger system-wide announcements or feature updates without touching the technical dashboard.
- **Support & Ops Teams** — quickly verify if a specific broadcast was successfully processed and delivered to users.
- **Developers** — test notification payloads, categories, and overrides directly from your code editor during development.


## Available Tools
- **create_broadcast**: Create a new broadcast
- **get_broadcast**: Fetch a specific broadcast
- **list_broadcasts**: List all broadcasts in the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MagicBell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent broadcasts in my MagicBell project."

**🤖 AI Agent:**
> I've retrieved the broadcasts for your project. You have 3 recent entries: 'Welcome Campaign' (ID: 8a2...), 'System Alert' (ID: 4f1...), and 'Weekly Digest' (ID: 9c2...). Which one would you like to inspect?

---

**👤 You:**
> "Show me the details and status for broadcast ID 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Inspecting broadcast 550e8400... The status is 'processed'. It was sent with the title 'Maintenance Notice' and reached 1,240 recipients across Email and Web Push channels.

---

**👤 You:**
> "Create a new broadcast titled 'Flash Sale' with content 'Get 50% off today only!' for all recipients."

**🤖 AI Agent:**
> I've successfully created the 'Flash Sale' broadcast. It is now being processed and triggered for your recipient list. You can track its progress using the generated ID: 771b92...


## Installation & Usage

To install and use the **MagicBell** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magicbell](https://vinkius.com/mcp/magicbell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

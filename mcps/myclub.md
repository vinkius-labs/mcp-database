# myClub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/myclub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/myclub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/myclub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Sports club management — manage members, events, and invoices via myClub.fi.

## Description
Connect your **myClub** account to empower your AI agents with club management capabilities. This server allows for seamless coordination of sports organizations and community activities.

### What you can do

- **Member Directory** — List and inspect member profiles and registration details
- **Event Coordination** — Monitor upcoming practices, games, and events
- **Billing Visibility** — Access club invoices and financial records programmatically
- **Achievement Tracking** — View member cards and earned merits within the club

### How it works

1. Subscribe to this server
2. Enter your **myClub API Token** and your club's **Subdomain**
3. Start managing your sports club directly from Claude, Cursor, or any MCP client


## Available Tools
- **get_event**: Get details for a specific event
- **get_invoice**: Get details for a specific invoice
- **get_member**: Get details for a specific member
- **list_cards**: List member cards
- **list_events**: List club events
- **list_invoices**: List club invoices
- **list_members**: List all club members
- **list_merits**: List club merits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **myClub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active members in the club."

**🤖 AI Agent:**
> Fetching members... I've found 45 active members. Here are the first few...

---

**👤 You:**
> "Show upcoming events for this month."

**🤖 AI Agent:**
> Retrieving events... You have a soccer practice on Friday and a tournament next Sunday.


## Installation & Usage

To install and use the **myClub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/myclub](https://vinkius.com/mcp/myclub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

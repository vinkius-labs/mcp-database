# BOSSDesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bossdesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bossdesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bossdesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your IT services via BOSSDesk — track tickets, assets, and users directly from any AI agent.

## Description
Connect your **BOSSDesk** ITSM account to any AI agent and orchestrate your IT support and asset management workflows through natural conversation.

### What you can do

- **Ticket Oversight** — List all support tickets and retrieve detailed history and requester metadata.
- **ITSM Automation** — Create and update tickets directly from your workspace to streamline incident reporting.
- **Asset Management** — Query and inspect hardware and software assets, including serial numbers and specifications.
- **User Coordination** — Access your employee directory and individual user profiles managed within the platform.
- **Location Tracking** — List and retrieve details for all physical office or site locations.
- **Communication** — Add public or private notes to tickets to maintain high team engagement.

### How it works

1. Subscribe to this server
2. Enter your BOSSDesk API Token and Subdomain
3. Start managing your IT services from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IT Managers** — quickly check ticket queues and asset availability without opening the BOSSDesk portal.
- **Help Desk Technicians** — monitor active cases and user details straight from their workflow tools.
- **System Administrators** — verify asset metadata and office locations using natural language.


## Available Tools
- **add_ticket_note**: Add a comment or note to a ticket
- **create_ticket**: Create a new support ticket
- **get_asset**: Get details of a specific asset
- **get_ticket**: Get details of a specific ticket
- **get_user**: Get details of a specific user
- **list_assets**: List all managed IT assets
- **list_locations**: List all physical locations
- **list_tickets**: List all IT support tickets
- **list_users**: List all system users
- **update_ticket**: Update an existing ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BOSSDesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open tickets in BOSSDesk."

**🤖 AI Agent:**
> I've retrieved your open tickets. You have 5 pending cases, including 'Broken Printer' (ID: 102) and 'New Laptop Request' (ID: 105). Which one would you like more details on?

---

**👤 You:**
> "Find the asset with serial number XYZ123."

**🤖 AI Agent:**
> I found the asset: Dell XPS 15 (ID: 502). It is currently assigned to John Doe and is in 'In Use' status. Its warranty expires in 6 months.

---

**👤 You:**
> "Add a note to ticket 102: 'Hardware ordered, waiting for delivery'."

**🤖 AI Agent:**
> Note successfully added to ticket 102. The status remains 'Waiting for Parts'.


## Installation & Usage

To install and use the **BOSSDesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bossdesk](https://vinkius.com/mcp/bossdesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

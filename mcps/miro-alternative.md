# Miro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miro-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/miro-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/miro-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Brainstorm, plan, and design together on an infinite visual canvas that brings distributed teams into the same creative space.

## Description
Connect your **Miro** account to any AI agent and simplify your visual collaboration and whiteboarding workflows through natural conversation.

### What you can do

- **Board Management** — List all collaborative boards, retrieve detailed metadata, and create new boards programmatically
- **Visual Content Control** — List all items on a board (sticky notes, shapes, text) and place new content directly from your agent
- **Member Coordination** — Query board members and sharing settings to manage access across your organization
- **Operational tracking** — Monitor board activity and stay on top of your visual projects
- **Direct Whiteboarding** — Add sticky notes and ideas to a board without leaving your conversation

### How it works

1. Subscribe to this server
2. Enter your Miro Access Token (OAuth 2.0)
3. Start managing your visual collaboration from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — organize roadmaps, sprint planning, and user journey maps visually.
- **Designers & UX Researchers** — manage board items, sticky notes, and brainstorming artifacts directly.
- **Agile Teams** — automate the creation of project boards and member synchronization.


## Available Tools
- **create_board**: Create a new Miro board
- **create_sticky_note**: Add a sticky note to a board
- **delete_board**: Delete a Miro board
- **get_board_details**: Get details for a specific board
- **list_boards**: List Miro boards
- **list_board_items**: List all items on a board
- **list_board_members**: List board collaborators
- **list_organizations**: List linked organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Miro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all boards in my Miro account."

**🤖 AI Agent:**
> I've retrieved your boards. You have access to: 'Product Roadmap Q4', 'User Interview Notes', and 'Brainstorming Session'. Which one should we open?

---

**👤 You:**
> "Add a sticky note with 'Implement SSO' to the 'Engineering' board."

**🤖 AI Agent:**
> Sticky note added! I've placed 'Implement SSO' on the 'Engineering' board (ID: uXjV...). You can check it now.

---

**👤 You:**
> "Who has access to the 'Confidential Strategy' board?"

**🤖 AI Agent:**
> Inspecting members... There are 4 users with access: Alex (Owner), Sarah (Editor), David (Viewer), and the Operations Team group.


## Installation & Usage

To install and use the **Miro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miro-alternative](https://vinkius.com/mcp/miro-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

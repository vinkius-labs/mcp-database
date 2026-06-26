# Miro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miro-alternative)
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


## Available Tools (8)
- **create_sticky_note**: Add a sticky note to a board
- **list_board_items**: List all items on a board
- **list_board_members**: List board collaborators
- **list_organizations**: List linked organizations
- **create_board**: Create a new Miro board
- **delete_board**: Delete a Miro board
- **get_board_details**: Get details for a specific board
- **list_boards**: List Miro boards


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


## ❓ FAQ

**Q: Can I list all items on a Miro board using my AI agent?**
Yes! Use the `list_board_items` tool and provide the Board ID. Your agent will retrieve all widgets, sticky notes, and text blocks on that board.

**Q: How do I add a new sticky note to a board?**
Use the `create_sticky_note` action. Provide the Board ID and the content of your note to place it programmatically on the whiteboard.

**Q: Is it possible to manage board members via AI?**
Yes, the `get_board_members` tool allows you to retrieve a list of all users who have access to a specific board, along with their roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miro-alternative](https://vinkius.com/mcp/miro-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Miro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `miro-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Miro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "miro-alternative": {
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

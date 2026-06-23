# Infinity Work Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infinity-work-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage work items, boards, comments, and folders via Infinity API.

## Description
Connect **Infinity** to any AI agent and manage your work management platform — create and update items, manage boards, add comments, organize folders, and track project progress through natural conversation.

### What you can do
- **Workspaces & Boards** — List and create workspaces and boards for organizing work
- **Item Management** — Create, update, and delete items with custom attribute values
- **Comments** — Add and retrieve comments on any item for collaboration
- **Folders** — Organize items into folders within boards
- **Attributes** — View board attribute configurations for custom fields
- **Profile** — Get authenticated user profile information

### How it works
1. Subscribe to this server
2. Enter your Infinity Access Token from Developer settings
3. Start managing work from Claude, Cursor, or any MCP-compatible client

Infinity is a highly customizable work management platform used by teams to organize projects, tasks, and workflows.

### Who is this for?
- **Project Managers** — Create and track work items without opening the web app
- **Team Leads** — Monitor board activity and add comments for team coordination
- **Operations Teams** — Manage folders and organize large volumes of work items efficiently


## Available Tools (15)
- **list_attributes**: List attributes configured on a board
- **list_boards**: Use board IDs to query items, folders, and attributes.

List all boards in a workspace
- **list_comments**: List comments on an item
- **create_board**: Body should include name and optional settings.

Create a new board in a workspace
- **create_comment**: Body should include content.

Add a comment to an item
- **create_folder**: Create a new folder in a board
- **create_item**: Body should include name and attribute values.

Create a new item in a board
- **delete_item**: Delete an item from a board
- **list_folders**: List folders in a board
- **get_board**: Get details of a specific board
- **get_item**: Get details of a specific item
- **list_items**: Supports pagination via cursor.

List all items in a board
- **get_profile**: Use this to verify connection and identify your user ID.

Get the authenticated user profile
- **update_item**: Update an existing item in a board
- **list_workspaces**: Use workspace IDs to query boards and items within specific workspaces.

List all workspaces accessible to the user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infinity Work Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all workspaces I have access to."

**🤖 AI Agent:**
> Found 3 workspaces: 1. Marketing Team. 2. Product Development. 3. Operations.

---

**👤 You:**
> "List all items in board 123 of workspace 456."

**🤖 AI Agent:**
> Found 15 items: 1. Design Homepage. 2. Update API Docs. 3. Fix Login Bug. 4. Launch Campaign.

---

**👤 You:**
> "Create a new item called 'Sprint Planning' in board 123 with status 'In Progress'."

**🤖 AI Agent:**
> Item created successfully! 'Sprint Planning' added to board 123 with status 'In Progress'.


## ❓ FAQ

**Q: How do I get my Infinity Access Token?**
Log in to Infinity, go to Profile > Developer Features, enable developer mode, and generate an Access Token in the Developer section.

**Q: Can I create items with custom attributes?**
Yes! Use the create_item action with a JSON body that includes the item name and attribute values matching your board configuration.

**Q: Can I add comments to items?**
Yes! Use the create_comment action with the workspace, board, and item IDs along with the comment content.

**Q: Can I manage multiple workspaces?**
Yes! You can list all your accessible workspaces and manage boards, folders, and items within each specific workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infinity-work-manager](https://vinkius.com/mcp/infinity-work-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infinity Work Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infinity-work-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infinity Work Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infinity-work-manager": {
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

# Miro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Miro boards, items and comments via API — create boards, add sticky notes, browse items and manage members from any AI agent.

## Description
Connect your **Miro** account to any AI agent and take full control of your visual collaboration through natural conversation.

### What you can do

- **Board Management** — List, create, update and inspect boards with their descriptions, owners and permissions
- **Item Operations** — Browse all widgets on a board (sticky notes, cards, shapes, texts, connectors, images) with their content and positions
- **Content Creation** — Create sticky notes and cards programmatically with custom content and canvas positions
- **Member Management** — List board members and add new users with specific roles (owner, admin, editor, commenter, viewer)
- **Comments** — Read and add comments on boards for async collaboration feedback

### How it works

1. Subscribe to this server
2. Enter your Miro Access Token (OAuth 2.0 or Personal Access Token)
3. Start managing your visual workspace from Claude, Cursor, or any MCP-compatible client

No more switching to the Miro app to check board content or add a quick sticky note. Your AI acts as a dedicated visual collaboration assistant.

### Who is this for?

- **Product Managers** — quickly review board contents, add meeting notes as sticky notes and track team feedback without opening Miro
- **Designers** — audit board items, review card contents and manage board membership for design reviews
- **Team Leads** — monitor collaboration activity, review comments and ensure proper board access for team members


## Available Tools (14)
- **add_board_member**: Requires the board ID and user ID. Optionally set the role (owner, admin, editor, commenter, viewer). The user must already have a Miro account.

Add a member to a Miro board
- **list_comments**: Each comment includes its ID, content text, author info, creation date and parent comment ID (for replies). Optionally set a limit.

List comments on a Miro board
- **create_board**: Requires the board name and optionally a description. Returns the created board with its ID, view link and edit link.

Create a new Miro board
- **create_card**: Requires the board ID and card title. Optionally set a description and x,y position. Cards are structured content widgets with title and description fields.

Create a card widget on a Miro board
- **create_comment**: Requires the board ID and comment content. Optionally reply to an existing comment by providing its ID as parent_id.

Add a comment to a Miro board
- **create_sticky_note**: Requires the board ID and the sticky note content (text). Optionally set the x,y position on the canvas. Returns the created sticky note with its ID and position.

Create a sticky note on a Miro board
- **delete_board_item**: Provide the board ID and item ID. WARNING: this action is irreversible.

Delete an item from a Miro board
- **get_board**: Provide the board ID (found in the board URL or from list_boards).

Get details for a specific Miro board
- **get_board_item**: Provide the board ID and item ID.

Get details for a specific item on a Miro board
- **get_user_context**: Returns user ID, name, email, avatar and account type. Use this to verify your access token is working correctly and to see which user identity the API calls will appear as.

Get the authenticated Miro user context
- **list_board_items**: ) placed on a Miro board. Each item includes its type, ID, content, position, rotation, size and style. Optionally filter by item type (sticky_note, card, shape, text, connector, image, embed, frame, document, mind_map) and set a limit.

List items (widgets) on a Miro board
- **list_board_members**: Each member shows their user ID, name, email, role (owner, admin, editor, commenter, viewer) and permission level. Optionally set a limit.

List members of a Miro board
- **list_boards**: Each board includes its ID, name, description, creation date, owner and permissions. Optionally set a limit on the number of results. Use this to discover boards before accessing their content.

List Miro boards accessible by the user
- **update_board**: Provide the board ID and the new name and/or description. Only provided fields will be updated.

Update a Miro board name or description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Miro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the sticky notes on my Sprint Planning board."

**🤖 AI Agent:**
> I found 12 sticky notes on your Sprint Planning board. Topics include: 'Implement OAuth flow', 'Fix checkout bug', 'Design new dashboard', 'Update API docs', 'Refactor auth middleware' and 7 more. Would you like the full content of any specific note?

---

**👤 You:**
> "Create a new board called 'Q2 OKRs' with a description 'Quarterly objectives and key results'."

**🤖 AI Agent:**
> Done! I've created the board 'Q2 OKRs' with the description. The board is ready for collaboration. Board URL: https://miro.com/app/board/uXjV... You can now add sticky notes, cards and other items to it.

---

**👤 You:**
> "Add a sticky note to my board saying 'Meeting notes: Discussed API versioning strategy' at position x:100, y:200."

**🤖 AI Agent:**
> Done! I've added the sticky note at position (100, 200) on your board with the text 'Meeting notes: Discussed API versioning strategy'. All board collaborators can see it immediately.


## ❓ FAQ

**Q: How do I get a Miro Access Token?**
Go to [**Miro Developer Portal**](https://developers.miro.com/), create an app, and generate a Personal Access Token (PAT) or set up OAuth 2.0. PATs are simpler for personal use — go to your app settings and create a token under 'Personal Access Tokens'. Copy it immediately as it won't be shown again.

**Q: Can I create sticky notes programmatically?**
Yes! Use `create_sticky_note` with the board ID and content text. Optionally set x,y coordinates on the canvas for precise positioning. The sticky note will appear on the board immediately and all collaborators will see it in real-time.

**Q: Can I manage board members via the API?**
Yes! Use `list_board_members` to see who has access and their roles, and `add_board_member` to grant access to new users with a specific role (owner, admin, editor, commenter, viewer). The user must already have a Miro account.

**Q: Can I filter board items by type?**
Yes! Use `list_board_items` with the type parameter to filter by: sticky_note, card, shape, text, connector, image, embed, frame, document, or mind_map. This is useful for finding specific widget types without loading all board content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miro](https://vinkius.com/mcp/miro)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `miro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Miro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "miro": {
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

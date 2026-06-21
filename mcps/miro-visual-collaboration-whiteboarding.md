# Miro (Visual Collaboration & Whiteboarding) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage collaborative boards via Miro — create sticky notes, list visual items, and audit team members.

## Description
Connect your **Miro** account to any AI agent and take full control of your visual collaboration, digital whiteboarding, and team ideation through natural conversation.

### What you can do

- **Board Orchestration** — List all accessible collaborative boards and retrieve detailed metadata including board titles and descriptions directly from your agent
- **Visual Content Injection** — Instantly create and attach new sticky notes or geometric shapes (rectangles, circles, triangles) to specific board coordinate grids securely
- **Canvas Audit** — List all distinct visual items physically attached inside a board, including text blocks and shapes, to understand the current state of your workspace
- **Team Collaboration** — Enumerate active team members sharing access across a specific board to verify direct viewer or editor permissions natively
- **Organizational Tags** — List semantic organizational tags applied inside a board to retrieve raw index groupings and manage project metadata efficiently
- **Project Provisioning** — Initialize fresh collaborative canvases on your active Miro account by creating brand new boards with custom titles and contextual overviews

### How it works

1. Subscribe to this server
2. Enter your Miro Access Token
3. Start managing your visual workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — organize roadmap ideas and track team feedback through natural conversation without manual board navigation
- **Designers & Researchers** — quickly log insights and attach sticky notes to research boards directly from your workspace
- **Engineering Teams** — audit collaborative board memberships and retrieve visual project summaries efficiently to maintain alignment


## Available Tools (8)
- **list_boards**: List high-level Miro Boards accessible globally
- **get_board**: Get static explicit configuration of a specific Miro Board
- **create_board**: Create a fresh new collaborative Miro Board
- **list_items**: ) nested within the designated Board ID string.

List raw items attached physically inside a Miro Board
- **create_sticky_note**: Create and attach a new sticky note component to a Board
- **create_shape**: Create and attach a geometric shape structure onto a Board
- **list_members**: List active team members sharing bounds across a Board
- **list_tags**: List semantic organizational tags applied inside a board


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Miro (Visual Collaboration & Whiteboarding)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Miro boards"

**🤖 AI Agent:**
> I've retrieved 3 boards from your Miro account: 'Product Roadmap Q1' (ID: 12345), 'UX Research: User Flow' (ID: 67890), and 'Sprint Retrospective' (ID: 13579). Which one would you like to inspect or add items to?

---

**👤 You:**
> "Create a sticky note on board '12345' with the text 'Review API auth flow'"

**🤖 AI Agent:**
> Sticky note created! I've successfully added 'Review API auth flow' to your 'Product Roadmap Q1' board. The item has been injected onto the canvas and is now visible to all collaborators.

---

**👤 You:**
> "Show me the tags used in the 'UX Research' board"

**🤖 AI Agent:**
> Retrieving tags… I've identified 4 semantic tags in the 'UX Research' board: 'High Priority', 'User Pain Point', 'Feature Request', and 'Follow-up Needed'. Would you like me to list the items associated with any of these tags?


## ❓ FAQ

**Q: Can I add a sticky note to a specific Miro board through my agent?**
Yes. Use the `create_sticky_note` tool by providing the Board ID and your text content. Your agent will inject a basic colored note onto the board's coordinate grid immediately, perfect for rapid ideation.

**Q: How do I see all the items currently on a board?**
The `list_items` tool retrieves all visual components physically attached to a board. Your agent will return a list of sticky notes, shapes, and text blocks, helping you audit the canvas content without opening the browser.

**Q: Can my agent list the team members who have access to my boards?**
Absolutely. Use the `list_members` tool with a specific Board ID. Your agent will report all active collaborators explicitly granted access, allowing you to verify viewer and editor permissions across your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding](https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Miro (Visual Collaboration & Whiteboarding)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `miro-visual-collaboration-whiteboarding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Miro (Visual Collaboration & Whiteboarding)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "miro-visual-collaboration-whiteboarding": {
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

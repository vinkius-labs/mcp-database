# Miro (Visual Collaboration & Whiteboarding) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/miro-visual-collaboration-whiteboarding-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/miro-visual-collaboration-whiteboarding-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Miro (Visual Collaboration & Whiteboarding)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding](https://vinkius.com/mcp/miro-visual-collaboration-whiteboarding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

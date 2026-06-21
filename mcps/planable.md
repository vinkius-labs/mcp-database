# Planable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/planable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/planable-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Collaborate, approve, and manage your social media content calendar autonomously using AI.

## Description
Connect your **Planable** workspaces directly to your AI agent to radically streamline your social media collaboration loops. You can review scheduled posts, approve mockups, respond to team comments, and oversee the content pipeline directly from your primary interface.

### What you can do

- **Workspace & Pages** — View active workspaces, team members, and all connected social accounts isolated in their respective boundaries.
- **Content Pipeline** — Retrieve post drafts, schedule future publications, and query statuses (draft, pending_approval, scheduled, published).
- **Approval Workflow** — Radically speed up content sign-off. Instruct your AI to transition posts from pending directly to approved, or formally reject them with custom revision notes.
- **Collaboration** — Add, fetch, and monitor chronological threaded comments on any isolated post.

### How it works

1. Subscribe to this Planable integration
2. Inject your Planable Enterprise API Key
3. Manage your social content engine using Claude, Cursor, or any MCP client

### Who is this for?

- **Social Media Managers** — bulk-schedule text content and respond to designer comments without opening browsers.
- **Marketing Directors** — quickly list all pending posts, read them out via the AI, and mass-approve the calendar.
- **Community Teams** — monitor scheduled outputs mapped onto federated social accounts easily.


## Available Tools
- **list_workspaces**: List Planable workspaces. Returns workspace IDs, names, and member counts. Planable is a social collaboration platform for content planning and approval
- **list_pages**: List social pages (connected accounts) in a Planable workspace. Returns page IDs, platform types, and display names
- **list_posts**: List posts in a Planable workspace by status. Returns post IDs, content previews, scheduled times, and approval status. Instructions: status = draft|pending_approval|approved|scheduled|published
- **get_post**: Get a Planable post by ID. Returns full content, media, schedule, approval history, and comments
- **create_post**: Create a Planable post. Instructions: Pass workspace_id, page_id, content text, and scheduled_at (ISO 8601). Post enters approval workflow
- **approve_post**: Approve a Planable post in the approval workflow. Moves it to scheduled status
- **reject_post**: Reject a Planable post with feedback. Returns it to draft for revisions
- **list_comments**: List comments on a Planable post. Returns comment IDs, authors, and text
- **add_comment**: Add a comment to a Planable post for team collaboration
- **list_workspace_members**: List members of a Planable workspace. Returns member IDs, names, emails, and roles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all posts in the 'Acme Marketing' workspace that are currently awaiting approval."

**🤖 AI Agent:**
> I found 4 posts marked `pending_approval`. The primary post (`ID: 29910`) is scheduled for tomorrow at 10 AM, targeting LinkedIn. The content reads: "We are excited to launch..." Would you like me to either directly approve this or insert a required revision comment?

---

**👤 You:**
> "Draft a new Twitter post in our workspace announcing our new AI feature."

**🤖 AI Agent:**
> Post created successfully via `create_post`. The underlying ID is `43109` mapped formally to the Twitter account logic array and deposited safely in draft status. Its exact body text generated: "Supercharge your endpoints with our revolutionary GenAI integration. Learn more today...".

---

**👤 You:**
> "Reject post `98341x` and tell the team to rewrite the hook, it's too salesy."

**🤖 AI Agent:**
> Understood. Sent the explicit mutation `reject_post` targeting `98341x`. I reversed the node state back into draft mode and attached the explicit feedback log: "Please rewrite the structural hook — it feels overly promotional and sales-oriented.". The content pipeline has been paused accordingly.


## Installation & Usage

To install and use the **Planable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planable](https://vinkius.com/mcp/planable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

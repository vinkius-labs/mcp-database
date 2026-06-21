# Planable MCP Server

Collaborate, approve, and manage your social media content calendar autonomously using AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/planable)

## Overview
**Category:** collaboration
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Planable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planable](https://vinkius.com/mcp/planable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

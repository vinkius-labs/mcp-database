# Frill MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frill)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/frill-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/frill-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage product feedback, roadmaps, and announcements via Frill — create ideas, list updates, and organize categories directly from your AI agent.

## Description
Connect **Frill** to your AI agent to streamline your product feedback loop and roadmap management through natural conversation.

### What you can do

- **Announcements & Changelogs** — List, create, and update product announcements to keep your users informed about new features.
- **Idea Management** — Capture user feedback by creating new ideas or querying existing ones using their unique IDX or slugs.
- **Categorization** — Organize your product updates with custom categories, including specific hex colors for visual consistency.
- **Roadmap Oversight** — Retrieve paginated lists of ideas and announcements to understand the current state of your product development.

### How it works

1. Subscribe to this server
2. Enter your Frill API Key
3. Start managing your product feedback and announcements from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — quickly draft announcements and review user ideas without switching tabs.
- **Customer Success Teams** — instantly check the status of a specific feature request or idea.
- **Developers** — update changelogs and announcement categories directly from the terminal or code editor.


## Available Tools
- **create_announcement**: Create a new announcement
- **create_category**: Create a new announcement category
- **create_comment**: Create a new comment on an idea
- **create_follower**: Create a new follower
- **create_idea**: Create a new idea
- **create_status**: Create a new status
- **create_topic**: Create a new topic
- **create_vote**: Vote on an idea
- **delete_announcement**: Delete an announcement
- **delete_category**: Delete an announcement category
- **delete_comment**: Delete a comment
- **delete_follower**: Delete a follower
- **delete_idea**: Delete an idea
- **delete_status**: Delete a status
- **delete_topic**: Delete a topic
- **delete_vote**: Unvote an idea
- **get_announcement**: Get a specific announcement
- **get_category**: Get a specific announcement category
- **get_idea**: Get a specific idea by IDX or slug
- **list_announcements**: List announcements in Frill
- **list_categories**: List announcement categories
- **list_comments**: List comments for an idea
- **list_followers**: List followers
- **list_ideas**: List ideas in Frill
- **list_statuses**: List statuses
- **list_topics**: List topics
- **list_votes**: List votes
- **search_followers**: Search followers by email
- **update_announcement**: Update an announcement
- **update_category**: Update an announcement category
- **update_comment**: Update a comment
- **update_follower**: Update a follower
- **update_idea**: Update an idea
- **update_status**: Update a status
- **update_topic**: Update a topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frill** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 announcements from Frill."

**🤖 AI Agent:**
> I've retrieved the latest 10 announcements. Recent updates include 'New Dashboard UI' (IDX: ann_1) and 'API v2 Release' (IDX: ann_2). Would you like to see the full content of any of these?

---

**👤 You:**
> "Create a new idea called 'Mobile App' with the description 'We need a native iOS and Android app'."

**🤖 AI Agent:**
> The idea 'Mobile App' has been successfully created with IDX 'idea_987'. It is now visible in your Frill feedback board.

---

**👤 You:**
> "Update the announcement 'ann_123' to set is_published to true."

**🤖 AI Agent:**
> Announcement 'ann_123' has been updated and is now published.


## Installation & Usage

To install and use the **Frill** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frill](https://vinkius.com/mcp/frill)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

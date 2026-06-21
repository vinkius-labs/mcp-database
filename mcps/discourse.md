# Discourse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discourse)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/discourse-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/discourse-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Equip your AI agent to manage forum topics, track community members, and monitor categories via the Discourse API.

## Description
Integrate **Discourse**, the open-source platform for community discussion, directly into your AI workflow. Manage your forum topics and categories, research community member profiles and trust levels, and track group memberships using natural language.

### What you can do

- **Discussion Oversight** — List and retrieve detailed information for the latest topics and trending discussions across your community.
- **Category Management** — Access the full category tree, resolving structural relationships and visibility settings.
- **Member Intelligence** — Research user profiles, track trust levels, and list active members in your organization.
- **Group Monitoring** — List community groups and identify all authorized members within specific group boundaries.

### How it works

1. Connect the Discourse integration to your AI assistant.
2. Authorize using your Discourse API Key, API Username, and instance URL.
3. Orchestrate your community management and discussions through intuitive conversation.

### Who is this for?

- **Community Managers** — Quickly check recent discussions and member activity on the go.
- **Moderators** — Research user history and trust levels via chat during moderation.
- **Content Strategists** — Monitor trending topics and category engagement to inform community planning.


## Available Tools
- **get_site_configuration**: Retrieve general settings and metadata for the Discourse instance
- **get_topic_details**: Get the full content and post list for a specific topic
- **get_user_profile**: Get detailed profile information for a specific user by username
- **list_active_members**: List currently active users in the community (admin access required)
- **list_forum_categories**: List all public categories available in the Discourse instance
- **list_group_members**: List all users belonging to a specific community group
- **list_community_groups**: List all user groups configured in the community
- **list_latest_topics**: List the most recent topics across all categories in the community
- **list_trending_discussions**: Identify topics with the highest engagement recently (mock logic)
- **search_community_content**: Search for topics, posts, or users matching a keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discourse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest topics in the community."

**🤖 AI Agent:**
> I've found several recent topics, including 'New Product Roadmap', 'Welcome to the Community', and 'Q2 Feedback Thread'. Would you like to see the post count for any of these?

---

**👤 You:**
> "Show me the profile for user 'john_doe'."

**🤖 AI Agent:**
> User 'john_doe' is at trust level 3 (Regular). They joined on January 15th and have created 12 topics and 45 posts. They are also a member of the 'Moderators' group. Should I check their recent activity?

---

**👤 You:**
> "What are the trending discussions right now?"

**🤖 AI Agent:**
> The top trending discussions are 'Major System Update' (25 new posts today) and 'Community Guidelines RFC' (12 new posts). Would you like a summary of the latest comments in 'Major System Update'?


## Installation & Usage

To install and use the **Discourse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discourse](https://vinkius.com/mcp/discourse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

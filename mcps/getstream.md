# GetStream MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getstream)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/getstream-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/getstream-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build and manage scalable activity feeds and social networks. Manage activities, feeds, and follower relationships directly through your AI agent.

## Description
Connect **GetStream** to your AI agent to orchestrate complex social architectures and activity feeds using natural language.

### What you can do

- **Feed Management** — Retrieve, add, or remove activities from specific feed slugs and user timelines using `get_feed` and `add_activity_to_feed`.
- **Activity Orchestration** — Update activity metadata or perform partial updates to specific fields via `partial_update_activity` without rewriting entire objects.
- **Social Graph** — Manage follower relationships, list who follows a feed, and perform follow operations using `follow_feed` and `list_feed_followers`.
- **Collections & Files** — Handle collection objects and manage file/image uploads for rich media experiences.
- **Open Graph** — Retrieve Open Graph data for URLs to enrich activity content automatically.

### How it works

1. Subscribe to this server
2. Enter your Stream API Key and JWT Token
3. Start managing your social infrastructure from any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor feed health and activity patterns without technical dashboards.
- **Developers** — test feed logic and activity updates directly from the IDE to speed up social feature integration.
- **Community Managers** — manage social graphs and moderate feed content through natural conversation.


## Available Tools
- **add_activity_to_feed**: Add an activity to a feed
- **add_to_collection**: Add objects to a collection
- **batch_delete_collections**: Batch delete collections
- **batch_follow**: Batch follow multiple feeds
- **batch_get_collections**: Batch retrieve collections
- **batch_post_collections**: Batch create/update collections
- **delete_collection_object**: Delete an individual collection object
- **delete_file**: Delete a file by URL
- **follow_feed**: Follow a target feed
- **get_activities**: Retrieve specific activities by ID or foreign ID
- **get_collection_object**: Retrieve an individual collection object
- **get_feed**: Supports pagination.

Retrieve activities in a feed
- **get_open_graph**: Scrape Open Graph data from a URL
- **list_feed_followers**: List feeds following this feed
- **list_feed_follows**: List feeds this feed follows
- **partial_update_activity**: Partially update activity data
- **process_image**: Process or resize an image
- **remove_activity_from_feed**: Remove an activity from a feed
- **unfollow_feed**: Unfollow a target feed
- **update_activities**: Update activity metadata
- **update_collection_object**: Update an individual collection object
- **upload_file**: Upload a file
- **upload_image**: Upload an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GetStream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest activities in the 'user' feed for user ID 'user_123'."

**🤖 AI Agent:**
> I've retrieved the feed for 'user:user_123'. There are 10 recent activities, including a post about 'New Product Launch' and a photo upload. Would you like to see the details of the most recent one?

---

**👤 You:**
> "Make the feed 'timeline:alice' follow 'user:bob'."

**🤖 AI Agent:**
> Successfully executed the follow command. 'timeline:alice' is now following 'user:bob'. Future activities from Bob will now appear in Alice's timeline.

---

**👤 You:**
> "Update activity ID 'act_999' to set the 'is_featured' field to true."

**🤖 AI Agent:**
> I have partially updated activity 'act_999'. The 'is_featured' field is now set to true. All other metadata remains unchanged.


## Installation & Usage

To install and use the **GetStream** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getstream](https://vinkius.com/mcp/getstream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

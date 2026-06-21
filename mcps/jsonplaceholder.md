# JSONPlaceholder MCP Server

Access fake online REST API for testing and prototyping — manage posts, comments, albums, photos, and todos directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jsonplaceholder)

## Overview
**Category:** productivity
**Tools Count:** 21

## Description
Connect to **JSONPlaceholder**, the industry-standard fake REST API, to simulate data interactions within your AI workflows. Perfect for developers testing MCP integrations or prototyping agentic behaviors without a real backend.

### What you can do

- **Post Management** — Use `list_posts`, `get_post`, `create_post`, `update_post`, `patch_post`, and `delete_post` to test full CRUD lifecycles.
- **Social Interactions** — Query comments via `list_comments` and `get_comment` to simulate discussion threads and linking.
- **Media Handling** — Explore `list_albums`, `get_album`, `list_photos`, and `get_photo` to manage hierarchical media metadata.
- **Task Tracking** — Use `list_todos` to verify state-based logic and completion status in your agents.
- **Data Filtering** — Test precise data retrieval by filtering lists by `userId`, `postId`, or `albumId` directly through tool parameters.

### How it works

1. Subscribe to this server
2. No real API key is required for this public service, but you can provide a placeholder string if prompted
3. Start prototyping your data-driven agents immediately

### Who is this for?

- **MCP Developers** — verify that your client correctly handles tool calls, pagination, and JSON responses
- **AI Researchers** — prototype complex agent behaviors that require structured data interaction without setting up a database
- **Product Designers** — demonstrate AI-driven workflows using realistic (but safe) mock data


## Available Tools
- **create_post**: Create a new post
- **delete_post**: Delete a post
- **get_album_photos**: Get photos for a specific album
- **get_album**: Get a specific album by ID
- **get_comment**: Get a specific comment by ID
- **get_photo**: Get a specific photo by ID
- **get_post_comments**: Get comments for a specific post
- **get_post**: Get a specific post by ID
- **get_todo**: Get a specific todo by ID
- **get_user_albums**: Get albums for a specific user
- **get_user_posts**: Get posts for a specific user
- **get_user_todos**: Get todos for a specific user
- **get_user**: Get a specific user by ID
- **list_albums**: Can be filtered by userId.

List all albums
- **list_comments**: Can be filtered by postId.

List all comments
- **list_photos**: Can be filtered by albumId.

List all photos
- **list_posts**: Can be filtered by userId.

List all posts
- **list_todos**: Can be filtered by userId.

List all todos
- **list_users**: List all users
- **patch_post**: Update a post (partial)
- **update_post**: Update a post (replace)


## Installation & Usage

To install and use the **JSONPlaceholder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsonplaceholder](https://vinkius.com/mcp/jsonplaceholder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# JSONPlaceholder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jsonplaceholder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access fake online REST API for testing and prototyping — manage posts, comments, albums, photos, and todos directly from your AI agent.

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


## Available Tools (21)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSONPlaceholder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all posts for user 1."

**🤖 AI Agent:**
> I've retrieved the posts for user 1. There are 10 posts available, including titles like 'sunt aut facere...' and 'qui est esse'. Would you like to see the full body of any specific post?

---

**👤 You:**
> "Get the details for comment ID 5."

**🤖 AI Agent:**
> Inspecting comment 5... It was posted by 'Hayden@althea.biz' with the body: 'harum non quasi et ratione...'. It is linked to post ID 1.

---

**👤 You:**
> "Create a new post for user 10 with title 'MCP Test' and body 'Testing JSONPlaceholder'."

**🤖 AI Agent:**
> Simulating post creation... Success! A new post has been 'created' with ID 101 for user 10. Title: 'MCP Test'. Note: Since this is a mock API, the data isn't permanently stored.


## ❓ FAQ

**Q: Can I filter posts by a specific user?**
Yes! Use the `list_posts` tool with the `userId` parameter to retrieve only the posts created by that specific user ID.

**Q: Does creating or updating a post actually save the data?**
No. JSONPlaceholder is a fake API. Tools like `create_post`, `update_post`, and `delete_post` simulate the response as if the action succeeded, but the server state remains unchanged.

**Q: How do I find comments for a specific post?**
Use the `list_comments` tool and provide the `postId`. This will return all comments associated with that specific post ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsonplaceholder](https://vinkius.com/mcp/jsonplaceholder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSONPlaceholder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jsonplaceholder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSONPlaceholder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jsonplaceholder": {
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

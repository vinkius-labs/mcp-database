# GoRest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gorest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access and manage RESTful data for users, posts, and comments via the GoRest API — perfect for testing, prototyping, and data simulation.

## Description
Connect to the **GoRest** API to interact with a full suite of RESTful resources. This server allows your AI agent to perform CRUD operations on users, posts, and comments, making it an essential tool for developers needing mock data or testing environments.

### What you can do

- **User Management** — List, fetch, create, update, and delete user profiles with specific attributes like gender and status.
- **Content Handling** — Manage blog-style posts and associated comments across the entire platform.
- **Data Filtering** — Query users by name, email, or status to find specific records quickly using advanced filtering.
- **Prototyping** — Use the API to simulate real-world application data flows within your AI-driven workflows.

### How it works

1. Subscribe to this server
2. Enter your GoRest Access Token
3. Start managing REST resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly populate UI components with realistic mock data without setting up a custom backend.
- **QA Engineers** — automate the creation and deletion of test users and posts to verify application logic.
- **Data Analysts** — practice querying and manipulating relational-style data structures through a simple REST interface.


## Available Tools
- **create_comment**: Requires authentication.

Add a comment
- **create_post_comment**: Requires authentication.

Add a comment to a specific post
- **create_post**: Requires authentication.

Create a new post
- **create_todo**: Requires authentication.

Create a new todo
- **create_user_post**: Requires authentication.

Create a post for a specific user
- **create_user_todo**: Requires authentication.

Create a todo for a specific user
- **create_user**: Requires authentication.

Create a new user
- **delete_post**: Requires authentication.

Delete a post
- **delete_user**: Requires authentication.

Delete a user
- **get_comment**: Fetch a single comment
- **get_post**: Fetch a single post
- **get_todo**: Fetch a single todo
- **get_user**: Fetch a single user
- **list_comments**: Supports pagination.

List all comments
- **list_post_comments**: Comments on a specific post
- **list_posts**: Supports pagination.

List all posts
- **list_todos**: Supports pagination.

List all todos
- **list_user_posts**: Posts authored by a specific user
- **list_user_todos**: Todos owned by a specific user
- **list_users**: List users
- **replace_user**: Requires authentication.

Replace a user (full)
- **update_post**: Requires authentication.

Update a post
- **update_user**: Requires authentication.

Update a user (partial)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoRest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 active female users from GoRest."

**🤖 AI Agent:**
> I've retrieved the users. Here are the first 10 active female profiles, including 'Aditi Sharma' (ID: 12345) and 'Meera Patel' (ID: 12346).

---

**👤 You:**
> "Create a new post for user 54321 with the title 'MCP Integration' and a short body text."

**🤖 AI Agent:**
> The post has been successfully created for user 54321. The new post ID is 98765.

---

**👤 You:**
> "Delete the user with ID 13579."

**🤖 AI Agent:**
> User 13579 has been successfully deleted from the system.


## ❓ FAQ

**Q: Can I filter users by their status or gender using this server?**
Yes! The `list_users` tool supports optional filters for `name`, `email`, `gender`, and `status`, allowing you to narrow down the results easily.

**Q: Is it possible to perform partial updates on a user profile?**
Absolutely. Use the `update_user` tool to modify specific fields like email or status without needing to provide the entire user object.

**Q: How can I view all comments across the platform?**
You can use the `list_comments` tool, which supports pagination to help you browse through all recorded comments in the system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gorest](https://vinkius.com/mcp/gorest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoRest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gorest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoRest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gorest": {
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

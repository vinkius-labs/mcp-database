# Dev.to (Forem) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devto-forem)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Dev.to and Forem articles — list posts, create content, and inspect user profiles directly from any AI agent.

## Description
Connect your **Dev.to** or **Forem** account to any AI agent and manage your technical writing and community presence through natural conversation.

### What you can do

- **Article Management** — List published articles, search by tags, and fetch specific posts by ID or path.
- **Content Creation** — Create new articles or update existing ones with full markdown support directly from your chat.
- **Personal Dashboard** — Access your own articles (published or drafts) and retrieve your authenticated user profile using `list_my_articles` and `get_me`.
- **Community Insights** — Look up other users with `get_user`, explore organization-specific content, and list organization members.
- **Moderation Tools** — Unpublish articles when necessary using `unpublish_article` (requires appropriate permissions).

### How it works

1. Subscribe to this server
2. Enter your Dev.to/Forem API Key
3. Start managing your blog posts and community interactions from Claude, Cursor, or any MCP client

### Who is this for?

- **Technical Writers** — draft and update articles without leaving your markdown editor or IDE.
- **Community Managers** — monitor organization posts and user profiles efficiently.
- **Developers** — automate the distribution of technical content and query community data via API.


## Available Tools (12)
- **create_article**: to/Forem. Requires API key.

Create a new article
- **get_article_by_id**: Get a single article by ID
- **get_article_by_path**: Get a single article by username and slug
- **get_me**: Get authenticated user details
- **get_user**: Get a user by ID or username
- **list_articles**: List published articles
- **list_my_articles**: Requires API key.

List authenticated user's articles
- **list_org_articles**: List organization's articles
- **list_org_users**: List organization's users
- **list_videos**: List articles with videos
- **unpublish_article**: Unpublishes a specific article.

Unpublish an article
- **update_article**: Requires API key.

Update an existing article


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dev.to (Forem)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 5 articles about 'javascript' on Dev.to."

**🤖 AI Agent:**
> I've retrieved the top articles for #javascript. Here are the most popular ones: 'Understanding Closures', 'ES2024 Features', 'Async/Await Guide'...

---

**👤 You:**
> "Create a new draft article titled 'My MCP Guide' with the content 'This is a test'."

**🤖 AI Agent:**
> Successfully created your draft 'My MCP Guide' (ID: 1829304). You can find it in your unpublished articles.

---

**👤 You:**
> "Show me my account details and API status."

**🤖 AI Agent:**
> I've fetched your profile using `get_me`. You are logged in as 'dev_writer_22' with ID 55432. Your API key is active and authorized.


## ❓ FAQ

**Q: Can I publish a new post directly from the chat?**
Yes! Use the `create_article` tool by providing a title and the markdown content. You can also set the `published` status to true or false for drafts.

**Q: How do I see my own drafts and published posts?**
You can use the `list_my_articles` tool. It allows you to filter by type, such as 'all', 'published', or 'unpublished' (drafts).

**Q: Can I look up another user's profile information?**
Yes, use the `get_user` tool with either their unique User ID or their username to retrieve their public profile details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devto-forem](https://vinkius.com/mcp/devto-forem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dev.to (Forem)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `devto-forem` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dev.to (Forem)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devto-forem": {
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

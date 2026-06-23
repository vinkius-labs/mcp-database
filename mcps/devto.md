# DEV.to MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your DEV.to presence — publish articles, fetch latest posts, and update content directly from your AI agent.

## Description
Connect your **DEV.to** account to any AI agent to streamline your technical writing and community engagement through natural conversation.

### What you can do

- **Article Publishing** — Create and publish new articles or save them as drafts directly from your conversation using Markdown.
- **Content Discovery** — Fetch the latest articles, search by specific tags, or retrieve detailed posts by ID or author path.
- **Personal Dashboard** — Access your own published and unpublished articles to manage your portfolio and track your contributions.
- **Updates & Moderation** — Update existing content, modify tags, or unpublish articles when necessary.
- **Community Insights** — Query rising or fresh content across the platform to stay updated with tech trends.

### How it works

1. Subscribe to this server
2. Enter your DEV.to API Key
3. Start managing your technical blog from Claude, Cursor, or any MCP-compatible client

No more switching between your editor and the browser to share your knowledge. Your AI acts as a technical editor and publishing assistant.

### Who is this for?

- **Technical Writers** — draft and publish articles directly from the environment where you write your code and notes.
- **Developers** — share snippets and tutorials on the fly without breaking your development flow.
- **DevRel & Community Managers** — monitor latest posts and manage organizational content efficiently.


## Available Tools (38)
- **create_article**: Requires authentication.

Publish a new article on DEV.to
- **create_listing**: Create a new listing
- **create_page**: Create a custom page (Admin only)
- **create_reaction**: Create a reaction to an article or comment
- **delete_page**: Delete a custom page (Admin only)
- **get_article_by_id**: Get an article by ID
- **get_article_by_path**: Get an article by username and slug
- **get_articles**: Get published articles
- **get_comment_by_id**: Get a comment by ID
- **get_comments**: Get comments for an article or podcast episode
- **get_followed_tags**: Get tags followed by the authenticated user
- **get_latest_articles**: Get latest articles
- **get_listing**: Get listing details by ID
- **get_listings_by_category**: Get listings filtered by category
- **get_listings**: List published listings (classifieds/ads)
- **get_me**: Get authenticated user details
- **get_my_all_articles**: Get both published and unpublished articles for the authenticated user
- **get_my_articles**: Get all articles for the authenticated user
- **get_my_published_articles**: Get published articles for the authenticated user
- **get_my_unpublished_articles**: Get unpublished articles (drafts) for the authenticated user
- **get_organization_articles**: Get articles published by an organization
- **get_organization**: Get organization details by username
- **get_organization_users**: Get users belonging to an organization
- **get_page**: Get details of a custom page (Admin only)
- **get_pages**: List all custom pages (Admin only)
- **get_podcast_episodes**: Get podcast episodes
- **get_profile_image**: Get profile image URL for a user or organization
- **get_reading_list**: Get the reading list for the authenticated user
- **get_tags**: Get a list of tags used on the platform
- **get_user**: Get a user by ID or username
- **get_videos**: Get articles that include a video
- **suspend_user**: Suspend a user (Admin only)
- **toggle_reaction**: Toggle a reaction to an article or comment
- **unpublish_article**: Unpublish an article (Admin/Moderator only)
- **unpublish_user**: Unpublish all articles and comments for a user (Admin only)
- **update_article**: Update an existing article
- **update_listing**: Update an existing listing
- **update_page**: Update a custom page (Admin only)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DEV.to** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest articles on DEV.to about 'typescript' and 'mcp'."

**🤖 AI Agent:**
> I've found several recent articles. The top ones are 'Building MCP Servers with TypeScript' and 'Advanced Type Safety in MCP'. Would you like to see the details for any of these?

---

**👤 You:**
> "Create a new draft article titled 'My First MCP Guide' with a short introduction."

**🤖 AI Agent:**
> I've created the draft for you. The article 'My First MCP Guide' is now saved in your DEV.to account with ID 1829304. You can find it in your unpublished articles.

---

**👤 You:**
> "Show me all my published articles so I can check their status."

**🤖 AI Agent:**
> Fetching your portfolio... You have 3 published articles: 'Understanding Webhooks', 'API Design Patterns', and 'The Future of MCP'. Which one would you like to inspect or update?


## ❓ FAQ

**Q: Can I create a draft without publishing it immediately?**
Yes! When using the `create_article` tool, simply set the `published` parameter to `false`. The article will be saved as a draft in your account.

**Q: How do I find my own articles that I haven't published yet?**
You can use the `get_my_unpublished_articles` tool. It will return a list of all your drafts currently stored on DEV.to.

**Q: Is it possible to update the tags or content of an existing post?**
Absolutely. Use the `update_article` tool with the specific article `id`. You can modify the title, body, tags, and other metadata fields.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devto](https://vinkius.com/mcp/devto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DEV.to** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `devto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DEV.to** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devto": {
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

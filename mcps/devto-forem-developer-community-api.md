# Dev.to (Forem Developer Community API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devto-forem-developer-community-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Dev.to presence — publish articles, track engagement, and interact with the developer community directly through AI.

## Description
Connect your **Dev.to** (Forem) account to your AI agent to streamline your technical writing and community management. This server provides full access to the Forem API, allowing you to handle content and community interactions without leaving your workspace.

### What you can do

- **Article Management** — Create, update, and list your articles. Manage drafts and published content with tools like `create_article` and `list_my_all_articles`.
- **Community Interaction** — Retrieve and manage comments using `list_comments`, and engage with content via `create_reaction`.
- **User & Org Insights** — Fetch profile data for users and organizations, list followers, and manage your reading list.
- **Content Discovery** — Search for articles by tags, popularity, or specific users using `list_articles` and `get_article_by_path`.
- **Admin & Moderation** — For authorized users, manage pages, display ads, and user status within a Forem instance.

### How it works

1. Subscribe to this server
2. Enter your Dev.to API Key (found in your account settings)
3. Start publishing and managing your developer community content from Claude, Cursor, or any MCP client

### Who is this for?

- **Technical Writers** — Draft and publish articles directly from your markdown editor.
- **Developer Advocates** — Monitor community feedback and respond to comments efficiently.
- **Content Marketers** — Track article performance and manage cross-posted content.


## Available Tools (36)
- **create_article**: Create a new article
- **create_display_ad**: Create a display ad
- **create_page**: Create a page
- **create_reaction**: Create a reaction
- **delete_page**: Delete page by ID
- **get_article_by_path**: Get article by username and slug
- **get_article**: Get article by ID
- **get_comment**: Get comment by ID
- **get_display_ad**: Get display ad by ID
- **get_me**: Get authenticated user profile
- **get_organization**: Get organization by username
- **get_page**: Get page by ID
- **get_profile_image**: Get profile image by username
- **get_user**: Get user by ID
- **list_articles**: List published articles
- **list_comments**: List comments
- **list_display_ads**: List display ads
- **list_followed_tags**: List followed tags for the authenticated user
- **list_followers**: List followers of the authenticated user
- **list_my_all_articles**: List all authenticated user's articles (published and unpublished)
- **list_my_articles**: List authenticated user's articles
- **list_my_published_articles**: List authenticated user's published articles
- **list_my_unpublished_articles**: List authenticated user's unpublished articles
- **list_organization_articles**: List organization's articles
- **list_organization_users**: List organization's users
- **list_pages**: List pages
- **list_podcast_episodes**: List published podcast episodes
- **list_reading_list**: List authenticated user's reading list
- **list_tags**: List tags used in the community
- **list_videos**: List articles with videos
- **suspend_user**: Suspend a user (Admin)
- **toggle_reaction**: Toggle a reaction
- **unpublish_article**: Unpublish an article (Admin/Moderator)
- **update_article**: Update article by ID
- **update_display_ad**: Update display ad by ID
- **update_page**: Update page by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dev.to (Forem Developer Community API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 5 articles about 'webdev' from the last 7 days."

**🤖 AI Agent:**
> I've found the top 5 articles for #webdev: 1. 'Modern CSS Techniques' by Jane Doe... [details]. Would you like me to summarize any of these?

---

**👤 You:**
> "Show me my unpublished drafts on Dev.to."

**🤖 AI Agent:**
> You have 3 unpublished drafts: 'Understanding MCP', 'Rust for Beginners', and 'API Design Tips'. Which one would you like to work on?

---

**👤 You:**
> "Get the latest comments for article ID 123456."

**🤖 AI Agent:**
> I've retrieved the comments for article 123456. There are 2 new comments: 'Great post!' from user123 and a question about implementation from dev_guru. Should I draft a reply?


## ❓ FAQ

**Q: Can I see both my published and unpublished articles?**
Yes! You can use `list_my_all_articles` to see everything, or use specific tools like `list_my_published_articles` and `list_my_unpublished_articles` to filter your content.

**Q: How do I find the top articles for a specific tag like 'javascript'?**
Use the `list_articles` tool and provide 'javascript' in the `tag` parameter. You can also use the `top` parameter to find the most popular ones over a certain number of days.

**Q: Can I manage my reading list through the AI?**
You can retrieve your reading list using the `list_reading_list` tool, allowing your AI to summarize or organize articles you've saved for later.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devto-forem-developer-community-api](https://vinkius.com/mcp/devto-forem-developer-community-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dev.to (Forem Developer Community API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `devto-forem-developer-community-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dev.to (Forem Developer Community API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devto-forem-developer-community-api": {
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

# Ghost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ghost-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Publish and monetize your content with a modern headless CMS built for newsletters, memberships, and independent creators.

## Description
Connect your **Ghost** publishing account to any AI agent and take full control of your content management and membership workflows through natural conversation.

### What you can do

- **Content Orchestration** — List and manage all blog posts (published, draft, scheduled) and retrieve detailed HTML content and metadata programmatically
- **Member Intelligence** — Query your subscriber directory and retrieve detailed profiles, including join dates and membership tiers to monitor audience growth
- **Site Navigation** — List and oversee static site pages (About, Contact) and manage content tags to maintain a perfectly organized site taxonomy
- **Publishing Control** — Create new posts or drafts and update publishing statuses directly through your agent to streamline your editorial pipeline
- **Site Visibility** — Retrieve general site settings, newsletter configurations, and active membership offers using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **Admin API Key** and **Admin Domain** from Ghost (Settings > Integrations > Custom Integration)
3. Start managing your digital publication from Claude, Cursor, or any MCP client

No more manual dashboard navigation to check post statuses or member counts. Your AI acts as your dedicated content strategist and site manager.

### Who is this for?

- **Content Managers** — instantly retrieve post details and manage drafts without opening the Ghost admin panel
- **Digital Publishers** — monitor membership tiers and verify newsletter configurations using natural language
- **Marketing Teams** — automate site settings querying to orchestrate cross-platform content strategies


## Available Tools (10)
- **list_members**: Includes emails, status, and join dates.

List all site members
- **list_newsletters**: Newsletters are used to send content updates to members.

List all configured newsletters
- **list_offers**: List active membership offers
- **list_pages**: g., About, Contact) defined on the Ghost site. Pages are similar to posts but used for non-blog content.

List all static site pages
- **list_posts**: Includes basic metadata and post IDs for detailed retrieval.

List all Ghost blog posts
- **list_tags**: Useful for organizing and filtering posts.

List all content tags
- **list_membership_tiers**: g., Free, Premium) available on the site. Useful for understanding the subscription structure.

List membership tiers and plans
- **create_post**: Requires a title and supports optional HTML content. The post is created as a "draft" by default but can be set to "published" immediately.

Create a new Ghost post or draft
- **get_post_details**: Essential for reviewing the full content of an article.

Get details for a specific post
- **get_site_settings**: Essential for verifying site identity.

Get Ghost site settings and configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ghost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my draft posts in Ghost."

**🤖 AI Agent:**
> I've retrieved your drafts. You have 3 posts in progress: 'AI Roadmap 2026', 'New Feature Launch', and 'Community Spotlight'. Would you like the full HTML content for any of these?

---

**👤 You:**
> "Create a new draft titled 'Welcome to our MCP Blog'."

**🤖 AI Agent:**
> Draft created! 'Welcome to our MCP Blog' is now live in your Ghost admin panel (ID: 654321). It is currently set to 'draft' status. Should I add some initial content for you?

---

**👤 You:**
> "Show me a list of all site members and their emails."

**🤖 AI Agent:**
> Fetching member directory... You have 150 registered members. Recent subscribers include 'Alice' (alice@example.com) and 'Bob' (bob@example.com). Would you like to check their membership tiers?


## ❓ FAQ

**Q: How do I find my Ghost Admin API Key?**
Log in to your Ghost admin panel, navigate to **Settings** > **Integrations**, click **Add custom integration**, and copy the Admin API Key and API URL.

**Q: What is the Admin Domain?**
It is the API URL provided in your custom integration settings (e.g., `https://your-site.ghost.io`). Do not include the `/ghost/api/admin/` part.

**Q: Can I publish a post immediately via AI?**
Yes! When using the `create_post` tool, set the `status` parameter to 'published' to make your content live instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghost-alternative](https://vinkius.com/mcp/ghost-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ghost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ghost-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ghost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ghost-alternative": {
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

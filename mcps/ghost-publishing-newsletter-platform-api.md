# Ghost (Publishing & Newsletter Platform API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ghost-publishing-newsletter-platform-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your Ghost publication — browse public content, manage posts, and automate your newsletter workflow directly from your AI agent.

## Description
Connect your **Ghost** CMS to any AI agent to streamline your publishing and content management workflows. This MCP server provides full access to both the Content API for public data and the Admin API for site management.

### What you can do

- **Content Discovery** — List public posts, authors, tags, and pages using powerful NQL filtering and pagination.
- **Post Management** — Create, update, and list posts (including drafts) directly through the Admin API tools.
- **Site Insights** — Retrieve global site settings, including titles, descriptions, and active membership tiers.
- **Newsletter Automation** — Orchestrate your content strategy by querying existing tags and authors to organize new drafts.

### How it works

1. Subscribe to this server
2. Enter your Ghost Admin Domain, Content API Key, and Admin Token
3. Start managing your publication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Quickly draft new posts and organize tags without leaving the chat interface.
- **Editors** — Review existing public content and site settings to ensure brand consistency.
- **Developers** — Query the Ghost API structure and metadata directly from the code editor to speed up theme or integration development.


## Available Tools (16)
- **admin_create_member**: Create a new member via Ghost Admin API
- **admin_create_post**: Create a new post via Ghost Admin API
- **admin_delete_post**: Delete a post via Ghost Admin API
- **admin_list_members**: Browse members via Ghost Admin API
- **admin_list_newsletters**: Browse newsletters via Ghost Admin API
- **admin_list_offers**: Browse subscription offers via Ghost Admin API
- **admin_list_pages**: Browse pages via Ghost Admin API
- **admin_list_posts**: Browse posts via Ghost Admin API
- **admin_list_webhooks**: Browse system webhooks via Ghost Admin API
- **admin_update_post**: Update an existing post via Ghost Admin API
- **content_list_authors**: Supports NQL filtering and pagination.

Browse or read public authors via Ghost Content API
- **content_list_pages**: Supports NQL filtering and pagination.

Browse or read public pages via Ghost Content API
- **content_list_posts**: Supports NQL filtering, pagination, and inclusion of related data.

Browse or read public posts via Ghost Content API
- **content_get_settings**: Fetch site settings via Ghost Content API
- **content_list_tags**: Supports NQL filtering and pagination.

Browse or read public tags via Ghost Content API
- **content_list_tiers**: Browse membership tiers via Ghost Content API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ghost (Publishing & Newsletter Platform API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 5 most recent public posts from my Ghost blog."

**🤖 AI Agent:**
> I've retrieved the latest posts. The most recent ones are 'The Future of AI', 'Ghost vs WordPress', and 'Mastering MCP'. Would you like to see the full content of any of these?

---

**👤 You:**
> "Create a new draft post titled 'Weekly Newsletter' with some placeholder HTML content."

**🤖 AI Agent:**
> Draft created successfully! The post 'Weekly Newsletter' (ID: 65f2a...) is now in your Ghost admin panel as a draft.

---

**👤 You:**
> "What are the active membership tiers on my site?"

**🤖 AI Agent:**
> I found 2 active tiers: 'Free' and 'Premium ($5/mo)'. Both are currently available for new signups.


## ❓ FAQ

**Q: Can I create and publish a new post directly using this integration?**
Yes! You can use the `admin_create_post` tool. You can specify the title, HTML content, and status (e.g., 'draft' or 'published') to manage your content lifecycle.

**Q: How do I filter posts by a specific tag or author?**
You can use the `filter` parameter in tools like `content_list_posts`. Ghost uses NQL (Netvibe Query Language), so you can pass strings like `tag:news` or `author:john` to narrow down your results.

**Q: Does this server support viewing private site settings?**
The `content_get_settings` tool retrieves public site settings like the title, description, and logo. For more sensitive administrative data, the Admin API tools provide access based on your provided Admin Token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghost-publishing-newsletter-platform-api](https://vinkius.com/mcp/ghost-publishing-newsletter-platform-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ghost (Publishing & Newsletter Platform API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ghost-publishing-newsletter-platform-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ghost (Publishing & Newsletter Platform API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ghost-publishing-newsletter-platform-api": {
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

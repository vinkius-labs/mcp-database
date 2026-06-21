# Ghost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ghost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage blog posts, track authors, and oversee static pages via AI agents with Ghost CMS.

## Description
Connect your **Ghost** publication to any AI agent to automate your content management workflows through the Model Context Protocol (MCP). Ghost is a powerful headless Node.js CMS tailored for modern publishing. This MCP server enables you to retrieve published posts, manage taxonomy tags, and fetch site configurations directly through natural conversation using the Ghost Content API.

### Key Features

- **Content Discovery** — List all published blog posts and static pages, retrieving detailed HTML content and metadata.
- **Taxonomy Oversight** — Retrieve and list all categorization tags to understand your content architecture.
- **Author Management** — Fetch profile details for active writers and contributors across the publication.
- **Site Configuration** — Access global settings, routing rules, and title schemas programmatically.
- **Subscription Insights** — Retrieve active membership tiers to understand paywall rules and pricing layers.
- **Real-time Synchronization** — Keep your headless CMS content accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Ghost Base URL and Content API Key (found in Integrations)
3. Start managing your publication from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Managers** — quickly retrieve published post data or list active authors without manual dashboard navigation.
- **Frontend Developers** — automate the retrieval of taxonomy tags and site configuration via simple AI commands.
- **Editorial Leads** — get a real-time overview of the static pages and subscription tiers active on the site.


## Available Tools
- **verify_api_connection**: Check connection
- **get_post_by_slug**: Get post details
- **get_author_details**: Get author profile
- **get_page_by_slug**: Get page details
- **get_site_settings**: Get site settings
- **get_tag_details**: Get tag metadata
- **list_subscription_tiers**: List subscription tiers
- **list_blog_authors**: List authors
- **list_static_pages**: List static pages
- **list_published_posts**: List published posts
- **list_content_tags**: List categories/tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ghost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 5 most recent published posts."

**🤖 AI Agent:**
> Retrieving posts... I found 5 recent articles, including 'Welcome to Ghost' and 'Writing with Markdown'. Would you like to read the full content of any of them?

---

**👤 You:**
> "Get the content of the post with the slug 'welcome'."

**🤖 AI Agent:**
> Fetching post... The post 'Welcome' was published on October 1st. The main content is: 'Welcome, it's great to have you here...'.

---

**👤 You:**
> "List all active subscription tiers."

**🤖 AI Agent:**
> Fetching tiers... Your publication has 2 active tiers: 'Free' ($0/month) and 'Premium' ($5/month).


## ❓ FAQ

**Q: How do I get a Content API Key for Ghost?**
Log in to your Ghost Admin dashboard, navigate to Settings > Integrations, and add a Custom Integration. You will find the Content API Key there.

**Q: Can I publish new posts using this integration?**
No, this integration uses the Content API which is read-only. It is designed to safely retrieve and query your published content.

**Q: What is the Base URL format?**
Your Base URL is the root domain where your Ghost site is hosted, for example: 'https://demo.ghost.io'. Do not include '/ghost/api/'.

**Q: How do I fetch related tags and authors for a post?**
Use the 'include' parameter in the 'get_post_by_slug' tool and pass the string 'tags,authors'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghost](https://vinkius.com/mcp/ghost)
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
3. Set Type to "SSE", enter `ghost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ghost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ghost": {
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

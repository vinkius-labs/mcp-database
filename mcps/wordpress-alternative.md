# WordPress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build and manage websites with the CMS that powers over 40 percent of the web through posts, pages, plugins, and themes.

## Description
Connect your **WordPress** site to any AI agent and simplify how you publish content, manage users, and organize your blog through natural conversation.

### What you can do

- **Content Publishing** — Create and manage blog posts and static pages with full HTML support and status control (publish, draft).
- **User Directory** — List and inspect site users, authors, and contributors to understand your editorial team.
- **Taxonomy Management** — List categories and tags used to organize your website content.
- **Content Maintenance** — Fetch detailed metadata for specific posts or delete unwanted content instantly via AI.
- **Remote Control** — Access your site's REST API to monitor activity without opening the WP Admin dashboard.

### How it works

1. Subscribe to this server
2. Enter your WordPress URL, Username, and Application Password
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Blogger & Content Creators** — quickly draft or publish articles and check post metadata via simple AI commands.
- **Site Administrators** — monitor user lists and manage site pages directly from the workspace.
- **Digital Agencies** — coordinate content updates and category organization across multiple client sites via AI.


## Available Tools
- **create_new_post**: Create a new blog post
- **delete_post**: Delete a blog post
- **get_post_details**: Get details for a specific post
- **list_blog_categories**: List blog categories
- **list_static_pages**: List static site pages
- **list_blog_posts**: List WordPress blog posts
- **list_site_users**: List site users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent blog posts on my site."

**🤖 AI Agent:**
> I've retrieved your latest posts. You have: 'Introduction to MCP', 'Why WordPress is King', and 'AI in Content Curation'. Which one would you like to inspect?

---

**👤 You:**
> "Create a draft post titled 'Benefits of Remote Work' with some placeholder text."

**🤖 AI Agent:**
> Success! The draft 'Benefits of Remote Work' has been created on your site (ID: 5521). You can find it in your WordPress dashboard under Posts > All Posts.

---

**👤 You:**
> "Who are the registered authors on my WordPress site?"

**🤖 AI Agent:**
> Fetching user list... I found 3 active users: 'admin' (Administrator), 'jane_doe' (Editor), and 'bob_smith' (Author). Let me know if you need details on any of them.


## ❓ FAQ

**Q: How do I create a new post as a draft?**
Use the `create_new_post` action. Provide the title and content, and set the optional status parameter to `draft`. The post will appear in your WP Admin for final review.

**Q: Can I see a list of all static pages like 'About Us'?**
Yes! Use the `list_static_pages` query. Your agent will retrieve all static pages from your WordPress site, including their IDs and current status.

**Q: Is it possible to delete a post via the AI?**
Absolutely. Use the `delete_post` tool and provide the unique ID of the post you want to remove. The content will be permanently deleted from your site.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-alternative](https://vinkius.com/mcp/wordpress-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WordPress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wordpress-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WordPress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wordpress-alternative": {
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

# BlogIn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blogin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Keep your team informed with internal blog posts, company updates, and knowledge sharing that everyone actually reads.

## Description
Connect your **BlogIn** internal blog to any AI agent and simplify how you share knowledge, track team updates, and manage your company's internal wiki through natural conversation.

### What you can do

- **Post Management** — List all internal blog posts and retrieve detailed metadata and HTML content for specific entries.
- **Content Creation** — Programmatically create new blog posts with titles, categories, and full text directly via AI.
- **Wiki & Pages** — Query static internal pages to access company policies, handbooks, and static documentation.
- **Team Directory** — List account users and members to understand your organizational structure and contributors.
- **Discussion Tracking** — Monitor recent comments across all posts to stay on top of internal feedback.
- **Categorization** — List and browse post categories to find relevant content by topic.

### How it works

1. Subscribe to this server
2. Enter your BlogIn API Key and Subdomain (found in your account settings)
3. Start managing your internal knowledge base from Claude, Cursor, or any MCP client

### Who is this for?

- **Internal Communicators** — quickly retrieve recent updates and publish new announcements via simple AI commands.
- **HR & Operations** — verify company policies and manage internal wiki pages directly from the workspace.
- **Team Leads** — monitor discussion comments and retrieve contributor profiles via the AI assistant.


## Available Tools (7)
- **create_internal_post**: Create a new blog post
- **get_post_details**: Get details for a specific post
- **list_categories**: List post categories
- **list_recent_comments**: List recent post comments
- **list_internal_pages**: List internal wiki pages
- **list_posts**: List BlogIn posts
- **list_team_members**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlogIn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent internal blog posts."

**🤖 AI Agent:**
> I've retrieved your latest posts. You have: 'New Office Policies', 'Team Lunch Recap', and 'Quarterly Roadmap Update'. Which one would you like to read the details for?

---

**👤 You:**
> "Show me the comments for the post 'Quarterly Roadmap Update'."

**🤖 AI Agent:**
> I've fetched the comments. There are 3 recent discussions including positive feedback from Sarah and a question from Mike about the timeline. Shall I retrieve the full text of the comments?

---

**👤 You:**
> "Create an internal post: 'New Benefits Guide' in the 'HR' category."

**🤖 AI Agent:**
> Success! The post 'New Benefits Guide' has been created in the 'HR' category (ID: cat_10293). It is now published and visible to your team members in BlogIn.


## ❓ FAQ

**Q: Can I see the HTML content of a specific internal post via AI?**
Yes! Use the `get_post_details` tool and provide the Post ID. Your agent will retrieve the complete metadata and HTML body for that specific blog entry.

**Q: How do I list all the static wiki pages in my account?**
Run the `list_internal_pages` query. The agent will retrieve a complete list of all static, wiki-style pages currently configured in your BlogIn account.

**Q: Is it possible to create a new internal post via AI?**
Absolutely. Use the `create_internal_post` action. Provide a title, the content, and an optional category ID to publish a new update instantly to your team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blogin](https://vinkius.com/mcp/blogin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BlogIn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blogin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BlogIn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blogin": {
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

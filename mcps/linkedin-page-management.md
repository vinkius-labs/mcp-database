# LinkedIn Page Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin-page-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Company Page posts, comments, and social actions via the LinkedIn REST API.

## Description
Connect your **LinkedIn Company Page** to any AI agent to automate your social media management and community engagement. This MCP server enables your agent to list managed organizations, publish new posts, moderate comments, and track social reactions directly from natural language interfaces.

### What you can do

- **Post Automation** — Publish text-based updates and commentary directly to your Company Page feed
- **Community Moderation** — List and retrieve comments on any post to stay engaged with your audience
- **Response Management** — Post official comments and replies on behalf of your organization to foster discussion
- **Social Analytics** — List likes and reactions on specific posts to monitor engagement trends
- **Content Maintenance** — Retrieve a history of organization posts and permanently remove outdated content
- **Organization Oversight** — Identify all pages where the authenticated user has management roles and ACLs

### How it works

1. Subscribe to this server
2. Enter your LinkedIn Access Token (with organization social scopes) and API Version
3. Start managing your Company Page from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — Automate posting schedules and community replies via natural language commands
- **Community Leads** — Quickly monitor reactions and moderate discussions without leaving your productivity tools
- **Marketing Developers** — Integrate social publishing and engagement tracking into your custom internal dashboards


## Available Tools (7)
- **list_post_comments**: List all comments on a specific post
- **create_post_comment**: Add a comment to a post as the organization
- **create_page_post**: Create a new post on a Company Page
- **delete_page_post**: Delete a specific post
- **list_post_likes**: List likes/reactions on a specific post
- **list_managed_pages**: Use this to find organization IDs.

List all LinkedIn Company Pages managed by the user
- **list_page_posts**: List recent posts from a Company Page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn Page Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all LinkedIn Company Pages I manage."

**🤖 AI Agent:**
> I've retrieved your managed pages. You have roles on 2 pages: 'Global Tech Solutions (ID: 12345)' and 'Creative Agency (ID: 67890)'.

---

**👤 You:**
> "Create a new post on page '12345' with the text 'Welcome to our weekly update!'."

**🤖 AI Agent:**
> Successfully published your post to Global Tech Solutions. The post URN is 'urn:li:share:987654321'.

---

**👤 You:**
> "Show comments for the post 'urn:li:share:987654321'."

**🤖 AI Agent:**
> I found 3 comments on that post. Highlights include a question from 'Jane Smith' about product availability and a thank you message from 'Robert Brown'.


## ❓ FAQ

**Q: Which scopes are required to post as an organization?**
Your access token must include `w_organization_social` to create posts and comments, and `r_organization_social` to list them.

**Q: How do I find my Organization ID?**
Use the `list_managed_pages` tool. It will return all organizations where you have management roles along with their unique IDs.

**Q: Can I reply to a specific comment?**
The current version supports creating top-level comments on posts. Support for threaded replies (using the `parent` field) is handled via the same comment tool by providing the parent URN if supported by the engine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin-page-management](https://vinkius.com/mcp/linkedin-page-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn Page Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin-page-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn Page Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin-page-management": {
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

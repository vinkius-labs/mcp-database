# Hashnode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hashnode)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Hashnode blog directly from your AI agent — fetch user profiles, read publication posts, and publish or update content.

## Description
Connect your **Hashnode** account to any AI agent to streamline your technical writing and blogging workflow. This MCP server allows you to interact with the Hashnode GraphQL API through natural language.

### What you can do

- **User Profiles** — Retrieve detailed information about any Hashnode user by their handle using `get_user`.
- **Publication Management** — List all posts from a specific publication using its domain or hostname with `get_publication_posts`.
- **Content Retrieval** — Fetch full post content and metadata using slugs and hostnames via `get_post`.
- **Publishing** — Create and publish new blog posts with Markdown support and custom tags using `create_post` directly from your conversation.
- **Editing** — Update existing posts, titles, and content with `update_post` without leaving your AI interface.

### How it works

1. Subscribe to this server
2. Enter your Hashnode Personal Access Token
3. Start managing your technical blog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Writers** — Draft and publish articles directly from your AI-assisted writing environment.
- **Developers** — Share knowledge and updates on your Hashnode blog without switching contexts.
- **Content Managers** — Monitor publication feeds and update existing posts efficiently.


## Available Tools (16)
- **update_post**: Modify an existing post
- **create_draft**: Requires Pro plan. If publicationId is omitted, auto-resolves from your publications.

Create a draft post without publishing
- **create_image_upload_url**: Content-Type must start with image/ (e.g., image/png). Max 8 MB. SVG rejected.

Get a presigned URL for uploading an image
- **create_post**: If publicationId is omitted, auto-resolves from your publications (1 blog = auto-select; 2+ = error listing options). Use get_my_publications to find your ID.

Publish a new post to a publication
- **delete_draft**: The author or publication admins can delete.

Soft-delete a draft
- **get_feed**: Use after cursor for pagination.

Get the global Hashnode feed
- **get_me**: Get the currently authenticated Hashnode user
- **get_my_publications**: Use this to find your Publication ID before creating posts or drafts.

List all publications owned by the authenticated user
- **get_post_by_id**: Get a single post by its ID
- **get_post**: Get a single post by its slug
- **get_publication_posts**: Get a list of posts from a specific publication
- **get_tag**: g., javascript, graphql).

Get details about a Hashnode tag
- **publish_draft**: The draft is soft-deleted after publishing.

Publish an existing draft as a post
- **submit_draft_for_review**: Used by contributors.

Submit a draft for editor review
- **update_draft**: All content fields are optional.

Update an existing draft
- **get_user**: Get details about a specific Hashnode user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hashnode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for Hashnode user 'johndoe'."

**🤖 AI Agent:**
> I've retrieved the profile for 'johndoe'. They are a Technical Writer with 1,200 followers and their blog is located at johndoe.hashnode.dev.

---

**👤 You:**
> "List all posts from the publication 'blog.hashnode.com'."

**🤖 AI Agent:**
> I found 10 recent posts on 'blog.hashnode.com'. The latest titles include 'Announcing New Features' and 'Markdown Guide for Developers'. Would you like to read the content of any of these?

---

**👤 You:**
> "Create a new post in publication '642f...' titled 'My MCP Guide' with content '# Introduction...'."

**🤖 AI Agent:**
> Successfully published your post 'My MCP Guide'! You can view it at your publication URL. The post ID is 65a2b...


## ❓ FAQ

**Q: Can I fetch profile details for any Hashnode user?**
Yes! Use the `get_user` tool with the specific username handle. The agent will return their profile information, bio, and social links.

**Q: Does the publishing tool support Markdown formatting?**
Absolutely. Both `create_post` and `update_post` accept `contentMarkdown`, allowing you to publish rich technical content with code blocks, headers, and links.

**Q: How do I list posts from a specific blog domain?**
Use the `get_publication_posts` tool and provide the `host` domain (e.g., 'engineering.hashnode.dev' or your custom domain). It will return a list of recent posts from that publication.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashnode](https://vinkius.com/mcp/hashnode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hashnode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hashnode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hashnode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hashnode": {
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

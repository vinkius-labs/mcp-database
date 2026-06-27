# LinkedIn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Publish to your personal profile or Company Page, share articles, react, comment, and manage LinkedIn engagement through your AI agent.

## Description
Transform your AI agent into a LinkedIn publishing powerhouse. This MCP server connects your AI workflow directly to the LinkedIn REST API, enabling you to publish as your personal profile or your Company Page, share articles with rich link previews, reshare content, react to updates, and engage in comment threads — all through natural conversation.

### What you can do

- **Personal & Company Page Publishing** — Post as yourself or as your Company Page. Every publishing tool supports an optional organization ID to switch between personal and page posting seamlessly.
- **Text Posts** — Publish original text posts to your LinkedIn feed with public visibility.
- **Article Sharing** — Share URLs with automatically generated link preview cards, including custom title and description.
- **Content Resharing** — Reshare existing LinkedIn posts with your own commentary to amplify reach.
- **Social Reactions** — React to any post using all six LinkedIn reaction types: Like, Celebrate, Support, Love, Insightful, and Funny.
- **Comment Engagement** — Post top-level comments on any LinkedIn post to join professional conversations.
- **Threaded Replies** — Reply directly to specific comments with nested responses for deeper discussions.
- **Profile Intelligence** — Retrieve your authenticated profile data including name, headline, photo, and profile URL.
- **Page Discovery** — List all Company Pages you administer to quickly find your organization ID.

### How it works

1. Subscribe to this server and enter your LinkedIn OAuth 2.0 credentials
2. Your agent resolves your identity automatically via the LinkedIn REST API
3. Start publishing, reacting, and commenting through natural language
4. To post as a Company Page, add the Community Management API product and include `w_organization_social` in your token scopes

### Who is this for?

- **Thought Leaders** — maintain a consistent publishing cadence without switching tools.
- **Marketing Teams** — distribute content across personal profiles and Company Pages as part of an automated workflow.
- **Community Builders** — engage with your network by reacting to and commenting on relevant posts.
- **Content Strategists** — manage your entire LinkedIn publishing pipeline from one interface.


## Available Tools (11)
- **delete_reaction**: Remove your reaction from a LinkedIn post
- **get_me**: Requires r_profile_basicinfo scope.

Get authenticated user profile from LinkedIn
- **comment_on_post**: The comment will appear as the authenticated user.

Comment on a LinkedIn post
- **create_post**: By default, posts as the authenticated user. To post as a Company Page, provide the organization_id (get it from list_organizations). Posting as a page requires w_organization_social scope.

Create a new text post on LinkedIn
- **delete_comment**: This action cannot be undone.

Delete a comment from a LinkedIn post
- **delete_post**: Works for both personal and Company Page posts. This action cannot be undone.

Delete a post from LinkedIn
- **list_organizations**: Returns organization IDs that can be used with the organization_id parameter in posting tools. Requires r_organization_social scope (Community Management API).

List LinkedIn pages you administer
- **react_to_post**: Supported types: LIKE, PRAISE (celebrate), APPRECIATION (support), EMPATHY (love), INTEREST (insightful), ENTERTAINMENT (funny).

React to a LinkedIn post
- **reshare_post**: To reshare as a Company Page, provide the organization_id. Posting as a page requires w_organization_social scope.

Reshare an existing LinkedIn post with your own commentary
- **create_article_post**: To post as a Company Page, provide the organization_id. Posting as a page requires w_organization_social scope.

Create a post with a link preview (article share)
- **reply_to_comment**: The parent comment URN format is: urn:li:comment:(urn:li:activity:{activityId},{commentId}).

Reply to a specific comment on a LinkedIn post (nested reply)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish a post on my LinkedIn: 'Excited to announce our latest product launch!'"

**🤖 AI Agent:**
> Post published successfully on your LinkedIn profile with public visibility. Your network will see it in their feed immediately.

---

**👤 You:**
> "Share this article on my LinkedIn with a comment: https://example.com/article"

**🤖 AI Agent:**
> Article shared on your LinkedIn profile with a rich link preview card. The post includes your commentary and the article will appear with its title and thumbnail.

---

**👤 You:**
> "Post this update as my Company Page: 'We just shipped v2.0 — here's what's new.'"

**🤖 AI Agent:**
> I found your Company Page and published the update under your organization profile with public visibility. Your page followers will see it in their feed.


## ❓ FAQ

**Q: Can I post as my Company Page instead of my personal profile?**
Yes. Every publishing tool (`create_post`, `create_article_post`, `reshare_post`) accepts an optional `organization_id` parameter. Use `list_organizations` to discover your page IDs, then include the ID when creating a post. This requires the Community Management API product with `w_organization_social` scope.

**Q: Can the agent publish posts with link previews?**
Yes. Use the `create_article_post` tool to share any URL with an automatically generated preview card. You can customize the title and description that appear alongside the link.

**Q: Can I reply to specific comments on a post?**
Yes. The `reply_to_comment` tool creates threaded replies under any comment. Provide the post URN, the parent comment URN, and your reply text to create a nested response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin](https://vinkius.com/mcp/linkedin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin": {
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

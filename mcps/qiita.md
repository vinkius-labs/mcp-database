# Qiita MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qiita)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Qiita presence — publish articles, discover trending topics, and engage with the Japanese developer community from your AI agent.

## Description
Connect your **Qiita** account to any AI agent to streamline your technical writing and community engagement on Japan's largest developer knowledge platform.

### What you can do

- **Article Publishing** — Create and publish new articles or save them as private drafts directly from your conversation using Markdown.
- **Content Discovery** — Search articles by keyword, tag, or author. Browse trending topics across the platform.
- **Personal Dashboard** — Access your own published articles, manage drafts, and track your contributions.
- **Social Engagement** — Follow/unfollow users and tags, like articles (LGTM), stock (bookmark) interesting posts, and post comments.
- **Community Insights** — Explore tags, discover popular topics, and analyze follower counts to optimize your content strategy.

### How it works

1. Subscribe to this server
2. Enter your Qiita Access Token
3. Start managing your Qiita presence from Claude, Cursor, or any MCP-compatible client

No more switching between your editor and the browser. Your AI acts as a technical editor and publishing assistant for the Japanese developer ecosystem.

### Who is this for?

- **Technical Writers** — draft and publish articles directly from where you code.
- **Developers targeting Japan** — share knowledge with Japan's largest developer community.
- **DevRel & Community Managers** — monitor trends and manage content across the Qiita platform.
- **International Teams** — publish bilingual content to reach both Japanese and global audiences.


## Available Tools (29)
- **delete_article**: This action cannot be undone. All associated comments, likes, and stocks will also be removed.

Permanently delete an article from Qiita
- **delete_comment**: This action cannot be undone. You can only delete comments you have authored.

Permanently delete a comment from Qiita
- **edit_comment**: You can only edit comments you have authored.

Update an existing comment on Qiita
- **follow_tag**: Articles with this tag will appear in your personalized feed. Following tags helps curate your content discovery experience.

Follow a tag on Qiita
- **follow_user**: Their new articles will appear in your feed. Following active community members helps discover quality content.

Follow a user on Qiita
- **get_article**: Use to analyze article structure, read full content, or prepare updates.

Get the full content of a single Qiita article by ID
- **get_comments**: Use for community feedback review, sentiment analysis, and engagement tracking.

Get all comments on a Qiita article
- **get_my_articles**: Use to audit your content performance, find articles to update, or review your publication history on the platform.

Get your own published articles on Qiita
- **get_my_profile**: Use to verify your identity, audit your community presence, or retrieve your user ID for further operations.

Get the authenticated user profile on Qiita
- **unfollow_tag**: Articles with this tag will no longer appear in your personalized feed.

Unfollow a tag on Qiita
- **get_tag_articles**: Use for content discovery within specific topics, competitive analysis, and trend monitoring within the Japanese developer community.

Get articles with a specific tag on Qiita
- **get_tag_detail**: Use to evaluate a tag before publishing or to analyze topic popularity.

Get details of a specific Qiita tag
- **get_tags**: Use for content strategy — understand which topics have the most engagement and readership on the Japanese developer platform.

Get popular tags on Qiita sorted by follower count
- **get_teams**: Qiita Team is the enterprise knowledge sharing platform for organizations.

Get Qiita Team organizations you belong to
- **get_user_articles**: Use for competitive analysis, content research, or auditing an author's publication history.

Get articles published by a specific Qiita user
- **get_user_followees**: Use for social graph analysis and understanding influence networks within the Qiita community.

Get users followed by a specific Qiita user
- **get_user_followers**: Use for audience analysis, engagement planning, and community growth tracking.

Get followers of a specific Qiita user
- **stock_article**: Stocked articles can be accessed from your profile page. Similar to saving/bookmarking a post.

Add an article to your stock (bookmarks)
- **get_user_stocks**: Use to understand a user's interests, discover curated content, or research what content resonates with specific community members.

Get articles stocked (bookmarked) by a specific user
- **get_user**: Use to research authors, verify identities, or analyze community influence.

Get a Qiita user profile by username
- **is_item_stocked**: Use to check bookmark status before toggling stock operations.

Check if an article is stocked (bookmarked) by you
- **like_article**: LGTM is Qiita's equivalent of a like/upvote. Liking articles boosts their visibility and signals appreciation to the author.

Like an article (LGTM)
- **post_comment**: Use for community engagement, providing feedback to authors, or contributing to technical discussions.

Post a comment on a Qiita article
- **publish_article**: Content is written in Markdown format. Provide up to 5 tags. Set private to true to create a limited-sharing article instead of a public one. Tags should be comma-separated.

Publish a new article on Qiita
- **search_articles**: Use the query parameter with Qiita search syntax: "tag:python", "user:username", "title:keyword", "created:>2024-01-01". Combine filters freely. Results include LGTM count, stock count, and comment count for engagement evaluation.

Search Qiita articles by keyword, tag, or user
- **unfollow_user**: Their articles will no longer appear in your feed.

Unfollow a user on Qiita
- **unlike_article**: The article's like count will decrease by one.

Remove like (LGTM) from an article
- **unstock_article**: The article itself is not affected.

Remove an article from your stock (bookmarks)
- **update_article**: You can modify the title, body, tags, or visibility. Use to fix typos, update content, change tags, or toggle public/private status.

Update an existing article on Qiita


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qiita** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest articles on Qiita about 'MCP' and 'AI agents'."

**🤖 AI Agent:**
> I've found several recent articles on Qiita about MCP and AI agents. The top ones include discussions about building MCP servers in TypeScript and integrating AI agents into development workflows. Would you like to see details for any of these?

---

**👤 You:**
> "Create a new article on Qiita titled 'Getting Started with MCP Servers' with a brief introduction."

**🤖 AI Agent:**
> I've published the article 'Getting Started with MCP Servers' on your Qiita account. It's now live and accessible to the community.

---

**👤 You:**
> "Show me my published articles on Qiita."

**🤖 AI Agent:**
> Here are your published articles on Qiita. You have 5 articles, with the most recent being 'Advanced TypeScript Patterns'. Would you like to update or manage any of them?


## ❓ FAQ

**Q: Can I create a private article without publishing it to the community?**
Yes! When using the `create_item` tool, set the `private` parameter to `true`. The article will be accessible only via direct link.

**Q: How do I search for articles about a specific technology?**
Use the `get_items` tool with the `query` parameter. Qiita supports advanced search syntax like `tag:python`, `user:username`, and date filters like `created:>2024-01-01`.

**Q: What is the LGTM feature and how do I use it?**
LGTM (Looks Good To Me) is Qiita's equivalent of a 'like'. Use the `like_item` tool with the article ID to express appreciation for quality content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qiita](https://vinkius.com/mcp/qiita)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qiita** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qiita` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qiita** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qiita": {
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

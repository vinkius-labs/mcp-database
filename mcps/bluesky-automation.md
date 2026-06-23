# Bluesky Automation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bluesky-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Full-spectrum Bluesky automation — 20 tools for publishing, engagement, analytics, social listening, and lead generation via the AT Protocol.

## Description
Connect your **Bluesky** account to your AI agent and unlock the most powerful AT Protocol automation available.

### 20 Tools — Full Network Control

- **Publishing** — Publish posts with automatic rich text (clickable links, @mentions, #hashtags) and link card previews with OG metadata.
- **Quote Posts** — Cite any post with your own commentary for maximum thought-leadership engagement.
- **Engagement** — Like, reply, repost, and quote posts. All replies include automatic link cards and facets.
- **Engagement Analytics** — Every post returns like count, reply count, and repost count for data-driven decisions.
- **Social Listening** — Search the entire network by keyword, sort by relevance or recency, and monitor trending topics in real time.
- **Lead Generation** — Search users by keyword, extract follower/following graphs, and qualify prospects via detailed profile analysis.
- **Timeline Intelligence** — Read your home timeline, any user's feed, custom algorithm feeds, and full conversation threads.
- **Community Management** — Follow, unfollow, mute users. Get notifications for mentions, replies, and likes.
- **Content Moderation** — Delete your own posts when needed.

### How it works

1. Subscribe to this server
2. Navigate to Bluesky **Settings > Advanced > App Passwords** to create a secure token.
3. Input your Handle and App Password.
4. Start automating your social strategy from Claude, Cursor, or any MCP client.

### Who is this for?

- **Founders & Creators** — Maintain an active presence and find early adopters for your products.
- **Marketing Teams** — Automate community engagement and monitor brand mentions at scale.
- **Developer Advocates** — Find technical discussions and assist developers directly on the timeline.


## Available Tools (20)
- **get_notifications**: Priority channel for defensive community management.

Get notifications (mentions, replies, etc) for the authenticated user
- **follow_user**: Follow a Bluesky user by their handle
- **get_timeline**: Get the authenticated user timeline
- **like_post**: ) of the post. If you do not have the URL/URI, use search_posts or get_author_feed to find it first.

Like a specific post on Bluesky using its public URL
- **publish_post**: Keep text under 300 characters. Links and hashtags are automatically parsed.

Publish a new top-level post to your Bluesky profile
- **repost**: ) of the post to share it on your own profile. If you do not have the URL/URI, use search_posts or get_author_feed to find it first.

Repost (retweet) a specific post on Bluesky
- **delete_post**: Provide the full public URL or the AT Protocol URI (at://...) of your post to execute deletion.

Delete a post you previously made on Bluesky
- **get_author_feed**: Get the timeline/feed of a specific Bluesky user
- **get_custom_feed**: Provide the full AT URI of the custom feed generator.

Get posts from a specific Bluesky custom feed/algorithm
- **mute_user**: Critical for timeline curation.

Mute a specific Bluesky user
- **get_trending_topics**: Get the current trending topics on Bluesky
- **unfollow_user**: Useful for curating your timeline or eliminating inactive accounts.

Unfollow a Bluesky user
- **get_followers**: Pair with get_profile to qualify prospects.

Get a list of users following a specific Bluesky handle
- **get_follows**: Get a list of users that a specific Bluesky handle is following
- **get_post_thread**: Read this to analyze the thread environment before engaging. Provide the full public URL or the AT Protocol URI (at://...) of the target post.

Get the full conversation/thread of replies for a specific post
- **get_profile**: Get a Bluesky user profile details
- **quote_post**: Provide the public URL or AT URI of the post to quote. More effective than plain repost for thought leadership and engagement.

Quote a post on Bluesky with your own commentary
- **reply_to_post**: ) of the post. If you do not have the URL/URI, use search_posts or get_author_feed to find it first. Read the thread context via get_post_thread before engaging.

Reply to a specific post on Bluesky
- **search_posts**: Sort by "top" for viral trends, or "latest" for real-time engagement.

Search Bluesky network for posts matching specific keywords
- **search_users**: Search for Bluesky users by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bluesky Automation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the top 10 posts about 'Model Context Protocol' on Bluesky sorted by engagement."

**🤖 AI Agent:**
> I found the top posts about MCP. The most engaged has 47 likes, 12 replies, and 8 reposts from @developer.bsky.social: 'Just built my first MCP server — game changer.' Would you like me to quote this post with your commentary?

---

**👤 You:**
> "Quote this post https://bsky.app/profile/user.bsky.social/post/abc1234 with the comment 'This is exactly why we built Vinkius.'"

**🤖 AI Agent:**
> Done! Your quote post is live with the embedded original post and your commentary. The link is clickable and the author will be notified.

---

**👤 You:**
> "Publish a post about our new security features with a link to https://vinkius.com/mcp/security-audit-prover"

**🤖 AI Agent:**
> Your post is live! The URL appears as a clickable link with a rich preview card showing the page title and description. Here is the direct link to your post.


## ❓ FAQ

**Q: How do I create an App Password?**
Log into your Bluesky account on the web or mobile app, navigate to **Settings > Advanced > App Passwords**, and click 'Add App Password'. Name it 'MCP Server' and use the generated password.

**Q: Will my main Bluesky password be safe?**
Yes. This MCP server explicitly requires an App Password, which provides scoped access without exposing your main account credentials. You can revoke this App Password at any time from your Bluesky settings.

**Q: Do links in posts appear clickable?**
Yes. All posts automatically detect URLs, @mentions, and #hashtags and convert them into rich text facets — the AT Protocol standard for clickable elements. Posts with URLs also include a link card preview with the page's title and description.

**Q: Is there a character limit for the posts?**
Yes, Bluesky enforces a strict 300-character limit per post. Your AI agent is instructed to automatically keep all published text within this limit, ensuring your posts are never rejected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bluesky-automation](https://vinkius.com/mcp/bluesky-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bluesky Automation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bluesky-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bluesky Automation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bluesky-automation": {
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

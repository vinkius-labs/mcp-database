# Bluesky Automation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bluesky-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Automate social listening, lead generation, and engagement on the Bluesky (AT Protocol) network directly from your AI agent.

## Description
Connect your **Bluesky** account to your AI agent and take full control of your social media operations. 

### What you can do

- **Social Listening** — Programmatically search for relevant conversations and discover emerging trends across the AT Protocol network.
- **Lead Generation** — Monitor specific keywords to find potential clients and engage with them at exactly the right moment.
- **Automated Publishing** — Publish content, threads, and updates seamlessly through your agent.
- **Conversational Engagement** — Reply to posts and like content without manually browsing the app, maintaining context in your AI workspace.

### How it works

1. Subscribe to this server
2. Navigate to Bluesky **Settings > Advanced > App Passwords** to create a secure token.
3. Input your Handle and App Password.
4. Start automating your social strategy from Claude, Cursor, or any MCP client.

### Who is this for?

- **Founders & Creators** — Maintain an active presence and find early adopters for your products.
- **Marketing Teams** — Automate community engagement and monitor brand mentions.
- **Developer Advocates** — Find discussions about specific technologies and assist developers directly on the timeline.


## Available Tools (19)
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
- **get_followers**: Pair with get_profile to qualify prospects.

Get a list of users following a specific Bluesky handle
- **get_follows**: Get a list of users that a specific Bluesky handle is following
- **get_post_thread**: Read this to analyze the thread environment before engaging. Provide the full public URL or the AT Protocol URI (at://...) of the target post.

Get the full conversation/thread of replies for a specific post
- **get_profile**: Get a Bluesky user profile details
- **get_trending_topics**: Get the current trending topics on Bluesky
- **mute_user**: Critical for timeline curation.

Mute a specific Bluesky user
- **reply_to_post**: ) of the post. If you do not have the URL/URI, use search_posts or get_author_feed to find it first. Read the thread context via get_post_thread before engaging.

Reply to a specific post on Bluesky
- **search_posts**: Sort by "top" for viral trends, or "latest" for real-time engagement.

Search Bluesky network for posts matching specific keywords
- **search_users**: Search for Bluesky users by keyword
- **unfollow_user**: Useful for curating your timeline or eliminating inactive accounts.

Unfollow a Bluesky user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bluesky Automation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find 10 recent posts discussing 'Model Context Protocol' on Bluesky."

**🤖 AI Agent:**
> I found several recent posts discussing the Model Context Protocol (MCP). Here is one from @developer.bsky.social: 'Just built my first MCP server to connect Claude with my local database! Game changer.' Would you like me to like this post or reply to them?

---

**👤 You:**
> "Publish a new post announcing our Vinkius AI marketplace launch."

**🤖 AI Agent:**
> Your post has been successfully published to Bluesky! It is now live on your profile. Here is the direct link: https://bsky.app/profile/vinkius.bsky.social/post/3abcdefg

---

**👤 You:**
> "Like and reply to this post: https://bsky.app/profile/user.bsky.social/post/abc1234 saying 'Great feature!'"

**🤖 AI Agent:**
> I've successfully liked the post and added your reply 'Great feature!' to the thread. The author will be notified of your interaction.


## ❓ FAQ

**Q: How do I create an App Password?**
Log into your Bluesky account on the web or mobile app, navigate to **Settings > Advanced > App Passwords**, and click 'Add App Password'. Name it 'MCP Server' and use the generated password.

**Q: Will my main Bluesky password be safe?**
Yes. This MCP server explicitly requires an App Password, which provides scoped access without exposing your main account credentials. You can revoke this App Password at any time from your Bluesky settings.

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

# Instagram (Social Media & Business) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/instagram-social-media-business)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Instagram presence via AI — publish photos and reels, analyze insights, and manage comments.

## Description
Connect your **Instagram Business** account to any AI agent and take full control of your social media content and audience engagement through natural conversation.

### What you can do

- **Content Publishing** — Dispatch professional photos and high-impact reels directly from your agent, including custom captions and automated scheduling flows
- **Audience Insights** — Query deep performance metrics for your posts and stories to understand reach, impressions, and engagement trends in real-time
- **Comment Management** — List, retrieve, and respond to customer comments on your media items to maintain a high-touch social presence effortlessly
- **Media Inventory** — Enumerate your published content library and extract detailed metadata, including permalinks and media types (IMAGE, VIDEO, CAROUSEL)
- **Profile Audit** — Access your Business account profile data and monitor follower counts and account biographies securely
- **Token Management** — Refresh long-lived access tokens directly through your agent to ensure uninterrupted service connectivity

### How it works

1. Subscribe to this server
2. Enter your Instagram Access Token and Business Account ID
3. Start managing your Instagram presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — publish content and monitor engagement metrics through natural conversation without jumping between mobile and desktop apps
- **Marketing Operations** — audit account insights and manage high-volume comment responses across multiple business profiles
- **Business Owners** — get rapid summaries of recent post performance and respond to top customer queries efficiently


## Available Tools (10)
- **get_profile**: Returns: username, display name, biography, followers, following, post count, website, profile picture, account type. For posts/media, use instagram.media. For post performance, use instagram.insights.

Get the authenticated Instagram account profile: username, bio, follower count, following, post count, website
- **get_media**: Returns media_type, caption, permalink, like_count, comments_count, timestamp. For post performance metrics, use instagram.insights with the media_id. For comments, use instagram.comments with the media_id.

Get recent Instagram posts — images, videos, reels, carousels — with like and comment counts
- **get_insights**: Requires a media_id — get it from instagram.media first. Only works for Business and Creator accounts. Returns: impressions (total views including repeats), reach (unique accounts), likes, comments, shares, saves.

Get performance insights for an Instagram post: impressions, reach, likes, comments, shares, saves, and total interactions
- **get_comments**: Requires a media_id — get it from instagram.media first. To reply to a comment, use instagram.comment.reply. To delete a comment, use instagram.comment.delete.

Get comments on an Instagram post — text, username, timestamp, like count, and reply count
- **get_media_children**: Requires a media_id.

Get all photos/videos within an Instagram carousel album
- **publish_photo**: The image_url MUST be a publicly accessible HTTPS URL — Instagram fetches it directly. Only works for Business and Creator accounts. For videos/reels, use instagram.publish.reel. ALWAYS confirm with the user before publishing. This action is irreversible.

Publish a photo to Instagram — provide a public image URL and caption
- **publish_reel**: The video_url MUST be a publicly accessible HTTPS URL pointing to an MP4 file. Only works for Business and Creator accounts. For photos, use instagram.publish.photo. ALWAYS confirm with the user before publishing. This action is irreversible.

Publish a Reel to Instagram — provide a public video URL and caption
- **reply_comment**: Requires a comment_id.

Reply to an Instagram comment
- **delete_comment**: Requires a comment_id.

Delete an Instagram comment
- **refresh_token**: Can be called any time after the token has been active for at least 24 hours. After refreshing, ALWAYS show the new access token and instruct the user to update their INSTAGRAM_ACCESS_TOKEN credential in Vinkius. The old token becomes invalid.

Refresh your Instagram access token — extends validity for another 60 days


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Instagram (Social Media & Business)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish this photo to Instagram with caption 'Enjoying the sunset! #vibes': https://example.com/photo.jpg"

**🤖 AI Agent:**
> Publishing photo… Container created successfully. Media ID: 178412345. Your photo is now live on Instagram! Would you like the permalink to share it elsewhere?

---

**👤 You:**
> "Show me the insights for my last 3 posts"

**🤖 AI Agent:**
> I've retrieved insights for your last 3 posts. Post 1 ('New Collection'): 1,240 reach, 45 saves. Post 2 ('Sale Event'): 3,500 reach, 120 saves. Post 3 ('Behind the Scenes'): 890 reach, 15 saves. Post 2 is performing exceptionally well with a 4.5% engagement rate.

---

**👤 You:**
> "Are there any new comments on the 'Product Launch' Reel?"

**🤖 AI Agent:**
> Yes, I found 5 new comments on your 'Product Launch' Reel. Highlights include: 'Love this!', 'When will it be available?', and 'Great color options'. Would you like me to draft replies for these?


## ❓ FAQ

**Q: Can I publish a Reel using my AI agent?**
Yes. Use the `publish_reel` tool. You just need to provide a public URL for the video and your caption. Your agent will handle the container creation and final publishing to your Instagram Business profile instantly.

**Q: How do I see performance metrics for a specific post?**
Ask your agent to `get_media_insights` for a specific Media ID. You'll receive deep metrics like reach, impressions, saved counts, and engagement rate directly in your chat interface.

**Q: Can my agent help me respond to comments?**
Absolutely. Use the `get_media_comments` tool to list recent feedback, and then use `reply_to_comment` to send your response. This allows you to manage community interaction without opening the Instagram app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/instagram-social-media-business](https://vinkius.com/mcp/instagram-social-media-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Instagram (Social Media & Business)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `instagram-social-media-business` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Instagram (Social Media & Business)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "instagram-social-media-business": {
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

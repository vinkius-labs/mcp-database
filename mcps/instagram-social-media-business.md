# Instagram (Social Media & Business) MCP Server

Manage your Instagram presence via AI — publish photos and reels, analyze insights, and manage comments.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/instagram-social-media-business)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Instagram (Social Media & Business)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/instagram-social-media-business](https://vinkius.com/mcp/instagram-social-media-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Mastodon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mastodon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate social interactions on the Fediverse — post statuses, manage follows, and track trending content directly from your AI agent.

## Description
Connect your **Mastodon** account to any AI agent and manage your decentralized social presence through natural conversation.

### What you can do

- **Status Management** — Post new toots, reply to threads, and manage visibility settings (public, unlisted, private, direct) using `post_status`.
- **Engagement** — Favorite, bookmark, and reblog content to interact with your community effortlessly.
- **Timeline Discovery** — Access your home timeline, public feeds, or specific tag streams to stay updated on the latest discussions.
- **Account Control** — Follow or unfollow users, manage blocks and mutes, and update your profile metadata directly.
- **Trending Insights** — Query trending tags, links, and statuses to understand what's happening across the instance.

### How it works

1. Subscribe to this server
2. Enter your Mastodon Personal Access Token
3. Start interacting with the Fediverse from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Schedule or draft posts and engage with followers without leaving your workflow.
- **Social Researchers** — Analyze trending topics and public timelines using AI-driven queries.
- **Community Managers** — Monitor notifications and manage account relationships efficiently.


## Available Tools (32)
- **clear_notifications**: This is irreversible. Use with caution.

Clear all notifications at once
- **unfollow_account**: Their posts will no longer appear in your home timeline.

Unfollow a user by account ID
- **bookmark_status**: Unlike favouriting, the post author is NOT notified. Use to save interesting posts you want to revisit later.

Save a post privately for later reference
- **get_trending_links**: Use to understand what external content the community is discussing — valuable for finding conversations around specific news or topics.

View external articles and links being shared the most right now
- **mute_account**: Their posts will be hidden from your timelines and notifications without unfollowing or blocking them.

Mute a user by account ID
- **reblog_status**: Equivalent to a retweet. Use to amplify content you want to endorse. Requires the status ID from a previous tool result.

Boost (share) a post to your followers
- **create_app**: Returns client_id and client_secret for the OAuth flow. Only needed once per application — not for posting or reading content.

Register a new OAuth application on the Mastodon instance
- **delete_status**: Cannot delete posts by other users. Use only for correcting mistakes on your own posts.

Delete one of your own posts by status ID
- **dismiss_notification**: Does not undo the action that caused it.

Dismiss a single notification
- **favourite_status**: The post author receives a notification. Use to acknowledge or endorse content. Requires the status ID from a previous tool result.

Like a post to show appreciation
- **block_account**: They will not be able to see your posts or interact with you. Use only for spam, harassment, or abusive accounts.

Block a user by account ID
- **check_health**: Returns OK if the server is up. Use to verify connectivity before performing actions.

Check if the Mastodon instance is online and responding
- **follow_account**: Their posts will appear in your home timeline. Use after discovering an interesting account through search, timelines, or notifications. Requires the account ID.

Follow a user by account ID
- **get_account_statuses**: Use when you want to see what a specific user has been posting recently. Requires the account ID — get it from search results, timeline posts, or notifications.

List recent posts by a specific account
- **get_account**: Returns display name, username, bio, follower/following counts. Use when you need details about a specific user after finding their account ID from a post or search.

Retrieve a user profile by account ID
- **get_home_timeline**: This is your personalized feed. Use to discover what the people you follow are discussing right now.

View your home feed — posts from accounts you follow
- **get_instance_info**: Use to understand the community size and focus of the instance.

Get instance metadata — name, description, user counts
- **get_instance_rules**: Read these before interacting to ensure compliance with community guidelines.

View the rules of the Mastodon instance
- **get_list_timeline**: Lists are curated groups of accounts. Use when you have a pre-configured list of accounts to monitor.

View posts from a curated list of accounts
- **get_notifications_v1**: Use to discover who is interacting with you and respond to mentions.

View your recent notifications — mentions, follows, favourites, boosts
- **post_status**: There is no other way to send content — if you want to reply to someone, you MUST call this tool. To reply to an existing post, set "in_reply_to_id" to the status ID of the post you are replying to. To create an original post, omit "in_reply_to_id". The "status" parameter is the full text content you want to publish. Never compose text without calling this tool — text only exists on Mastodon after this tool is called.

Publish or reply on Mastodon. This is the ONLY way to send a message
- **register_account**: Requires an approved OAuth application first. Most instances require manual admin approval after registration.

Register a new user account on the Mastodon instance
- **get_public_timeline**: This is the broadest discovery tool — shows posts from all users across all connected instances. Use when you want to find new conversations and people to interact with.

View the public timeline — recent posts from all users
- **get_trending_statuses**: These are posts with high organic engagement. Use to find popular conversations where your reply will have maximum visibility and impact.

View posts that are trending right now
- **get_notifications_v2**: Only available on Mastodon 4.3 or newer instances. Falls back to v1 if the instance does not support v2.

View grouped notifications (Mastodon 4.3+)
- **search**: Use to find specific conversations, users, or topics. Set "type" to narrow results: "statuses" for posts, "accounts" for users, "hashtags" for tags. Without a type filter, returns all three. This is the primary discovery tool for finding content to interact with.

Search for accounts, posts, or hashtags by keyword
- **update_credentials**: Does not affect posting or interactions.

Update the authenticated account profile
- **verify_credentials**: Use this to confirm identity before performing actions.

Check if credentials are valid and get the authenticated account profile
- **get_status_context**: Use when you want to understand the full discussion before replying to a post.

Fetch the full conversation thread for a post
- **get_status**: Use when you need to read a post before replying to it, or to verify the content of a post found in timelines or search results.

Fetch a single post by its status ID
- **get_tag_timeline**: Use to find conversations about a specific topic. Pass the hashtag without the # symbol (e.g. "AI" not "#AI"). Great for discovering posts about specific technologies, events, or communities.

View recent posts containing a specific hashtag
- **get_trending_tags**: Mastodon trends are algorithm-free and purely based on real usage, making them a reliable signal of genuine community interest. Use to discover active topics for engagement.

View hashtags that are trending right now


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mastodon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Post a new status saying 'Hello from my AI agent!' with public visibility."

**🤖 AI Agent:**
> I've posted your status using `post_status`. It is now live on your profile with public visibility.

---

**👤 You:**
> "Show me the top 5 trending tags on this instance."

**🤖 AI Agent:**
> Fetching trends... The top tags currently are #Technology, #Art, #Fediverse, #News, and #Photography.

---

**👤 You:**
> "Verify my account and show my profile details."

**🤖 AI Agent:**
> Credentials verified! Your account is '@user@instance.social', with 150 followers and 200 following. Your bio is currently set to 'AI Enthusiast'.


## ❓ FAQ

**Q: Can I post a status with a content warning (spoiler text)?**
Yes. When using the `post_status` tool, you can provide a `spoiler_text` string which will act as a content warning for your followers.

**Q: How do I verify if my access token is working correctly?**
You can use the `verify_credentials` tool. It will test your current token and return your authenticated profile information if successful.

**Q: Is it possible to see what is currently trending on my instance?**
Absolutely. Use the `get_trending_tags` tool to retrieve the most popular hashtags used on your instance recently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mastodon](https://vinkius.com/mcp/mastodon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mastodon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mastodon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mastodon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mastodon": {
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

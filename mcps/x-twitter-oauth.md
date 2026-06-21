# X (Twitter) OAuth MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/x-twitter-oauth)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/x-twitter-oauth-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/x-twitter-oauth-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Full read and write access to X (Twitter) via OAuth 2.0 — post tweets, like content, follow users, browse timelines, track mentions, and monitor trends directly from any AI agent.

## Description
Connect your **X (Twitter)** account to any AI agent via OAuth 2.0 and unlock full read and write capabilities.

### What you can do

#### Read
- **Your Profile** — Instantly retrieve your own account details, follower count, and bio
- **Recent Tweet Search** — Find discussions from the last 7 days using keywords, hashtags, or handles
- **User Lookups** — Fetch complete profile metadata for any public user by @username
- **Tweet Introspection** — Pull exact content and engagement metrics for any tweet by ID
- **User Timeline** — Browse a user's most recent original posts
- **Mention Tracking** — Monitor who is talking about or replying to a specific user
- **Followers** — Retrieve the follower list of any user with full profile details
- **Liked Tweets** — See what content a user has liked
- **Volume Analysis** — Get time-series tweet counts to spot trending spikes

#### Write
- **Post Tweets** — Publish new tweets or reply to existing ones
- **Delete Tweets** — Remove your own tweets
- **Like / Unlike** — Like or remove likes from any tweet
- **Follow / Unfollow** — Follow or unfollow any user
- **Retweet** — Amplify content by retweeting

### How it works

1. Subscribe to this server
2. Enter your X Developer App Client ID and Client Secret
3. Click "Connect" — authorize in the popup
4. Start managing your X presence from Claude, Cursor, or any MCP-compatible client

The Vinkius platform handles OAuth 2.0 PKCE, token refresh, and secure storage automatically.

### Who is this for?

- **Community Managers** — post updates, reply to mentions, and like key interactions without leaving the AI
- **Founders & Creators** — manage your personal brand from your development environment
- **Growth Teams** — follow strategic accounts, retweet partners, and audit competitor followers at scale


## Available Tools
- **get_user_liked_tweets**: Requires the user numeric ID.

Retrieve tweets that a specific user has liked
- **delete_tweet**: You can only delete your own tweets.

Delete a tweet from the authenticated account
- **follow_user**: Requires your own user ID and the target user ID. Use get_my_profile for your ID and lookup_user_by_username for theirs.

Follow another user from the authenticated account
- **get_my_profile**: Returns the user's name, bio, follower count, and numeric ID.

Retrieve the authenticated user's own X (Twitter) profile details
- **get_tweet_details**: Retrieve the text and engagement metrics of a specific Tweet by its numeric ID
- **get_tweet_volume**: Returns time-series buckets showing how many tweets match a query.

Get the volume of tweets matching a search query over the last 7 days, broken down by hour or day
- **get_user_followers**: Requires the user numeric ID. Returns up to 50 followers with their profiles.

Retrieve the followers of a specific user
- **like_tweet**: Requires both the authenticated user's numeric ID and the tweet ID. Use get_my_profile to find your user ID.

Like a tweet from the authenticated account
- **get_user_mentions**: Requires the user numeric ID.

Retrieve recent tweets that mention a specific user (public @mentions)
- **get_user_timeline**: Requires the user numeric ID, not the username. Use lookup_user_by_username first to get the ID, or use get_my_profile for the authenticated user.

Fetch the most recent original tweets posted by a specific user (excludes retweets and replies)
- **post_tweet**: Optionally provide a tweet ID to reply to. The text must be 280 characters or less.

Post a new tweet to X (Twitter) from the authenticated account
- **retweet**: Requires your user ID and the tweet ID.

Retweet a tweet from the authenticated account
- **search_recent_tweets**: Provide a search query string.

Search for recent public tweets (up to last 7 days) using keywords, hashtags, or handles
- **unfollow_user**: Unfollow a user from the authenticated account
- **unlike_tweet**: Remove a like from a tweet
- **lookup_user_by_username**: Do not include the "@" symbol.

Fetch full details of a specific X (Twitter) user by their @username


## 💬 Prompt Examples

Here are some examples of how you can interact with the **X (Twitter) OAuth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Post a tweet saying 'Just shipped our new AI integration — try it now!'"

**🤖 AI Agent:**
> Done! Tweet posted successfully with ID 1234567890. Your followers can now see it. Want me to check the engagement metrics in a few minutes?

---

**👤 You:**
> "Show me my latest mentions and like any positive ones."

**🤖 AI Agent:**
> You have 5 recent mentions. 3 are positive — I've liked all three. One is a question about pricing and another is neutral feedback. Want me to reply to the pricing question?

---

**👤 You:**
> "Follow @openai and check their latest tweets."

**🤖 AI Agent:**
> Done — now following @openai (ID: 4398626122). Their latest tweets discuss GPT-5 benchmarks and a new safety paper. Want me to retweet any of them?


## Installation & Usage

To install and use the **X (Twitter) OAuth** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/x-twitter-oauth](https://vinkius.com/mcp/x-twitter-oauth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# X (Twitter) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/x-twitter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/x-twitter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/x-twitter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate social intelligence workflows via X (Twitter) — search recent tweets, analyze volume trends, retrieve profiles individually or in batch, and inspect engagement metrics from any AI agent.

## Description
Connect your **X (Twitter)** developer account to any AI agent and take full control of your social listening workflow through natural conversation.

### What you can do

- **Recent Tweet Search** — Search for latest public discussions (up to past 7 days) across the network using exact keywords, hashtags, or handles
- **User Lookups** — Fetch precise profile metadata of a specific user by their @username, revealing follower counts, location, and biographies
- **Tweet Introspection** — Provide a raw Tweet ID and instantly collect isolated text content alongside full engagement metrics (likes, retweets, impressions)
- **Batch Tweet Lookup** — Fetch up to 100 tweets at once by their IDs in a single request for efficient bulk analysis
- **Batch User Lookup** — Compare multiple user profiles simultaneously by passing several @usernames in one call
- **Volume Analysis** — Get time-series tweet counts for any query, broken down by minute, hour, or day to spot trending spikes

### How it works

1. Subscribe to this server
2. Enter your X (Twitter) App Bearer Token
3. Start scanning social data securely from Claude, Cursor, or any MCP-compatible client

No need to scrape HTML or fiddle with complex Postman queries. Your AI agent becomes your eyes on the timeline.

### Who is this for?

- **Founders & Creators** — track brand mentions or specific niche keywords to respond early to sentiment shifts
- **Product Researchers** — pull lists of recent tweets about competitors and ask the agent to summarize common user pain points
- **Marketing Teams** — audit influencers' engagement by checking exact follower counts and most prominent tweets in seconds


## Available Tools
- **get_tweet_details**: Retrieve the text and engagement metrics of a specific Tweet by its numeric ID
- **get_tweet_volume**: Returns time-series buckets showing how many tweets match a query. Great for spotting spikes in brand mentions or trending topics.

Get the volume of tweets matching a search query over the last 7 days, broken down by hour or day
- **lookup_users_batch**: Pass usernames as a comma-separated string without the "@" symbol.

Fetch profile details of multiple X (Twitter) users at once by their @usernames (up to 100)
- **get_tweets_batch**: Pass IDs as a comma-separated string.

Retrieve text and engagement metrics for multiple tweets at once by providing their IDs (up to 100)
- **search_recent_tweets**: Provide a search query string.

Search for recent public tweets (up to last 7 days) using keywords, hashtags, or handles
- **lookup_user_by_username**: Do not include the "@" symbol.

Fetch full details of a specific X (Twitter) user by their @username (follower count, bio, location)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **X (Twitter)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for tweets mentioning 'Vinkius Cloud' over the last couple days."

**🤖 AI Agent:**
> I've fetched 8 recent tweets mentioning 'Vinkius Cloud'. The sentiment is mostly positive, praising the new LLM integrations. One user encountered a latency issue. Want me to summarize their exact complaint?

---

**👤 You:**
> "Look up the profile details for 'elonmusk'."

**🤖 AI Agent:**
> Profile fetched: Elon Musk is based in Austin, TX and currently has over 180M followers. His bio reads '...'. Should I retrieve his most recent tweets?

---

**👤 You:**
> "Get the engagement stats for tweet ID 123456789."

**🤖 AI Agent:**
> The tweet 'Just shipped the new API v2!' has 4,500 likes, 320 retweets, and 12 replies so far. The engagement rate seems healthy based on your average metrics.


## Installation & Usage

To install and use the **X (Twitter)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/x-twitter](https://vinkius.com/mcp/x-twitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

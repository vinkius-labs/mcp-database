# CrowdTangle MCP Server

Equip your AI agent to track public social media insights, viral posts, and link shares via the CrowdTangle API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdtangle)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Integrate **CrowdTangle**, the public insights tool from Meta, directly into your AI workflow. Monitor social media trends, track how links are being shared across platforms, and identify high-performing content using natural language.

### What you can do

- **Post Monitoring** — List and search for recent public posts on Facebook, Instagram, and other supported platforms.
- **Viral Discovery** — Identify overperforming and viral content based on actual vs. expected interaction.
- **Link Tracking** — See which public accounts and pages have shared specific URLs.
- **Leaderboards & Lists** — Monitor account leaderboards and manage your custom tracking lists.

### How it works

1. Connect the CrowdTangle integration to your AI assistant.
2. Authorize using your CrowdTangle API Token (found in your dashboard Settings).
3. Analyze public social media data and trends through intuitive conversation.

### Who is this for?

- **Journalists & Newsrooms** — Track breaking stories and monitor how news is spreading online.
- **Digital Marketers** — Identify viral trends and audit competitor engagement strategies.
- **Researchers** — Analyze public discourse and link sharing patterns across social platforms.


## Available Tools
- **get_account_details**: Touches dashboard settings, API rate limits, and workspace configuration boundaries.

Retrieve metadata for your CrowdTangle account
- **get_account_leaderboard**: Resolves account rankings, total interactions, and average engagement rates.

Get engagement leaderboard for accounts in your lists
- **get_link_shares**: Resolves which tracked accounts shared the link, their follower counts, and total interactions generated per share.

See which accounts have shared a specific URL
- **get_post_details**: Touches reaction breakdowns, share history, and platform-specific metadata boundaries.

Get full engagement details for a specific post ID
- **get_top_performing_posts**: Resolves "score" metrics (actual vs expected interactions) and associated social media metadata.

Get the highest performing posts based on actual vs. expected interaction
- **list_monitored_lists**: Resolves list IDs, names, platform affiliations, and the number of accounts within each list.

List all account lists you are tracking
- **list_media_posts**: Resolves media URLs, content types (Photo, Video), and associated post captions.

List recent posts that contain photos or videos
- **list_recent_posts**: Resolves post content, platform identifiers (Facebook, Instagram, etc.), account names, and engagement metrics (likes, shares, comments).

List recent social media posts tracked by CrowdTangle
- **search_tracking_lists**: Resolves list metadata matching the specified title filter.

Search for specific tracking lists by title
- **search_posts_by_keyword**: Resolves relevant posts, associated accounts, and comparative performance data.

Search for posts across platforms using a keyword


## Installation & Usage

To install and use the **CrowdTangle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdtangle](https://vinkius.com/mcp/crowdtangle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

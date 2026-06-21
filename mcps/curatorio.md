# Curator.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/curatorio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/curatorio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/curatorio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage social media feeds, monitor posts, and audit sources directly via the Curator.io API.

## Description
Integrate **Curator.io**, the modern social media aggregator, directly into your AI workflow. Manage your social feeds, monitor recent posts across multiple platforms, and audit your social media sources using natural language.

### What you can do

- **Feed Management** — List and retrieve detailed settings for all your aggregated social feeds.
- **Post Monitoring** — Track recent posts within specific feeds and monitor their status and interaction details.
- **Source Discovery** — List all social media sources (accounts, hashtags) associated with your feeds.
- **Moderation Oversight** — Access active moderation and filtering rules to ensure consistent content display.

### How it works

1. Connect the Curator.io integration to your AI assistant.
2. Authorize using your Curator.io API Key (found in your account settings).
3. Manage your social aggregation strategy through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check social feed statuses and recent post counts on the go.
- **Digital Strategists** — Audit social media sources and moderation rules via chat.
- **Content Curators** — Search for specific social posts within aggregated feeds for research and planning.


## Available Tools
- **get_account_details**: Resolves usage limits and account identifiers. Interacts with the account and billing boundary.

Retrieve metadata for your Curator.io account
- **get_feed_details**: Resolves moderation settings, design configurations, and metadata. Interacts with the feed configuration boundary.

Get detailed settings and metadata for a specific feed
- **get_feed_post_count**: Resolves quantitative feed metrics. Touches the data aggregation and metrics boundary.

Get the total number of posts currently in a feed
- **list_active_feeds**: Resolves operational feed records. Touches the feed status management boundary.

Quickly list only the feeds that are currently active
- **list_social_connections**: Resolves account identifiers and authentication states. Touches the OAuth and external API integration boundary.

List connected social media accounts (Instagram, Twitter, etc.)
- **list_social_feeds**: Resolves feed IDs, names, and current statuses. Interacts with the feed management system.

List all social media feeds configured in Curator.io
- **list_moderation_rules**: Resolves keyword filters and exclusion patterns. Touches the content moderation logic boundary.

List active moderation and filtering rules for a feed
- **list_feed_posts**: Resolves post content, timestamps, and source origin. Touches the content delivery and aggregation boundary.

List recent social media posts within a specific feed
- **list_feed_sources**: Resolves source types (Instagram, Twitter, etc.) and connection parameters. Touches the ingestion gateway boundary.

List all social media sources (accounts, hashtags) for a feed
- **search_posts_in_feed**: Resolves matching post entities. Touches the indexed content search boundary.

Search for specific social posts within a feed by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Curator.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active social feeds in my account."

**🤖 AI Agent:**
> I've found 3 active feeds: 'Company Instagram', 'Event Hashtag #Tech2024', and 'Customer Testimonials'. Would you like to see the recent posts for any of these?

---

**👤 You:**
> "Show me the last 5 posts from the 'Event Hashtag #Tech2024' feed."

**🤖 AI Agent:**
> I've retrieved the last 5 posts for '#Tech2024'. They include 3 photos from Instagram and 2 tweets. One post from 'user_alpha' is trending with high engagement. Should I provide the source URLs?

---

**👤 You:**
> "What are the social sources for my 'Company Instagram' feed?"

**🤖 AI Agent:**
> The 'Company Instagram' feed (ID: 456) is aggregating data from 2 sources: the official '@company_global' account and the '#WorkingAtCompany' hashtag. Would you like to check the moderation rules for these sources?


## Installation & Usage

To install and use the **Curator.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curatorio](https://vinkius.com/mcp/curatorio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

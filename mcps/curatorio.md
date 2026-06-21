# Curator.io MCP Server

Equip your AI agent to manage social media feeds, monitor posts, and audit sources directly via the Curator.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/curatorio)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Curator.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curatorio](https://vinkius.com/mcp/curatorio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

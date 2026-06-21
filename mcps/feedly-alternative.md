# Feedly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feedly-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feedly-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feedly-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stay ahead of industry trends by aggregating RSS feeds, tracking topics with AI, and organizing research in focused boards.

## Description
Connect your **Feedly** account to any AI agent and take full control of your news aggregation and content curation workflows through natural conversation.

### What you can do

- **Feed Orchestration** — List and manage your subscribed news sources programmatically, including adding or removing RSS/Atom feeds
- **Stream Intelligence** — Retrieve the latest entries (articles) from specific feeds or categories and monitor unread counts in real-time
- **Content Extraction** — Programmatically fetch complete article text and metadata to perform deep analysis and summaries via your agent
- **Organization Control** — Manage your Feedly categories and personal tags to maintain a structured and high-fidelity reading environment
- **Reading Workflow** — Mark articles as read and manage your reading list programmatically to streamline your news consumption

### How it works

1. Subscribe to this server
2. Retrieve your **Developer Access Token** from Feedly (Settings > Integrations > Developer Token)
3. Start managing your news curation from Claude, Cursor, or any MCP client

No more manual scrolling through endless articles. Your AI acts as your dedicated news analyst and content curator.

### Who is this for?

- **Market Researchers** — instantly track industry news and retrieve full article contents for deep analysis using natural language
- **Content Strategists** — monitor trending topics across specific feeds and manage curation tags without leaving your workspace
- **Busy Professionals** — automate the process of marking articles as read and summarizing daily highlights through simple AI queries


## Available Tools
- **subscribe_to_feed**: Follow a new news source
- **get_article_details**: Get full content of an article
- **get_feed_metadata**: Get metadata for a specific feed
- **get_user_profile**: Get your Feedly profile
- **get_stream_contents**: Retrieve articles from a stream
- **list_categories**: List your Feedly categories
- **list_subscriptions**: List all subscribed feeds
- **list_tags**: List your personal tags
- **mark_articles_as_read**: Mark one or more articles as read
- **unsubscribe_from_feed**: Stop following a news source


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feedly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my categories in Feedly."

**🤖 AI Agent:**
> I've retrieved your categories. You have 4 organized streams: 'Tech' (ID: user/.../category/Tech), 'AI & ML', 'Market News', and 'Design'. Which one should we check for new articles?

---

**👤 You:**
> "Show me the last 3 unread articles in the 'AI & ML' category."

**🤖 AI Agent:**
> Fetching unread articles from AI & ML... I've found 3 new entries, including 'New LLM Benchmarks' and 'The state of RAG'. Would you like the full text summaries for these?

---

**👤 You:**
> "Subscribe to this feed: 'https://example.com/rss' and add it to 'Tech'."

**🤖 AI Agent:**
> Done! I've successfully added the new feed to your Feedly account under the 'Tech' category. You'll now see articles from this source in your Tech stream.


## Installation & Usage

To install and use the **Feedly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feedly-alternative](https://vinkius.com/mcp/feedly-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

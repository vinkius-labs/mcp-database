# Substack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/substack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/substack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/substack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with direct access to Substack — manage publications, draft posts, and track subscriber data without opening the Substack editor.

## Description
Connect **Substack** to your AI agent and manage your newsletter publication conversationally.

### What you can do

- **Post Management** — List, create, and manage newsletter posts including drafts, published, and scheduled content.
- **Subscriber Insights** — Query subscriber counts, growth trends, and audience demographics.
- **Publication Settings** — Access and modify publication metadata, categories, and custom domains.
- **Content Analytics** — Track open rates, click rates, and engagement metrics per post.

### How it works

1. Subscribe to the Substack integration on the marketplace.
2. Get your API token from your Substack publication settings (Settings → Publication API).
3. Ask your AI agent to draft posts, check analytics, or manage subscribers.

### Who is this for?

- **Newsletter Creators** — Draft and schedule posts without switching context to the Substack editor.
- **Content Marketers** — Track newsletter performance and audience growth from a conversational interface.
- **Thought Leaders** — Manage multiple Substack publications efficiently from your AI workflow.


## Available Tools
- **list_posts**: List recent posts
- **get_post**: Get post
- **get_post_stats**: Get post stats
- **list_subscribers**: List subscribers
- **get_publication_info**: Get publication info
- **get_leaderboard**: Get leaderboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Substack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many subscribers does my Substack have?"

**🤖 AI Agent:**
> Your publication has 4,250 total subscribers. Breakdown: 3,890 free (91.5%) and 360 paid (8.5%). Growth this month: +185 new subscribers (4.5% growth rate). Churn: 12 unsubscribes.

---

**👤 You:**
> "Draft a new newsletter post titled 'The Future of AI in Sales'."

**🤖 AI Agent:**
> Draft created: 'The Future of AI in Sales'. Status: Draft (unpublished). You can ask me to add body content, set a subtitle, or schedule it for publication.

---

**👤 You:**
> "What was the open rate on my last newsletter?"

**🤖 AI Agent:**
> Your last newsletter 'Q1 Market Insights' had a 52% open rate (2,210 opens out of 4,250 sent), 8% click rate on embedded links, and generated 23 new subscribers from shares.


## Installation & Usage

To install and use the **Substack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/substack](https://vinkius.com/mcp/substack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Determ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/determ)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/determ-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/determ-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to monitor media mentions, track keywords, and analyze sentiment via the Determ (formerly Mediatoolkit) API.

## Description
Integrate **Determ** (formerly **Mediatoolkit**), the powerful media monitoring and social listening platform, directly into your AI workflow. Track brand mentions across the web and social media, analyze sentiment trends, and monitor your competitive landscape using natural language.

### What you can do

- **Mention Monitoring** — List and retrieve real-time media mentions for your keywords and topics from over 100 million sources.
- **Sentiment Intelligence** — Retrieve a breakdown of sentiment (positive, neutral, negative) for any of your monitoring queries.
- **Query Management** — List and review your configured monitoring queries and their specific settings.
- **Analytics Reporting** — Access metadata for your media monitoring and analytics reports directly via chat.

### How it works

1. Connect the Determ integration to your AI assistant.
2. Authorize using your Determ API Key (found in your settings).
3. Orchestrate your brand monitoring and reputation management through intuitive conversation.

### Who is this for?

- **PR & Communications Managers** — Quickly check recent mentions and brand sentiment on the go.
- **Marketing Teams** — Monitor campaign reach and identify top media sources via chat.
- **Social Media Specialists** — Track social listening queries and mention details during planning sessions.


## Available Tools
- **search_mentions_by_keyword**: Search for specific keywords within the mentions of a monitoring query
- **get_account_metadata**: Retrieve settings and limits for your Determ account
- **get_mention_details**: Get full content and technical metadata for a specific media mention
- **get_monitoring_query_details**: Get detailed settings and status for a specific monitoring query
- **get_query_sentiment_summary**: Retrieve a breakdown of sentiment (positive, neutral, negative) for a specific query
- **list_media_mentions**: List recent media mentions for a specific monitoring query
- **list_monitoring_queries**: List all media monitoring queries (keywords/topics) in your Determ account
- **list_recent_high_reach_mentions**: List only the mentions with the highest estimated reach
- **list_analytics_reports**: List all available analytics and media monitoring reports
- **list_top_media_sources**: Identify the media sources with the highest volume of mentions (mock logic)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Determ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active monitoring queries."

**🤖 AI Agent:**
> I've found 4 active queries in your account: 'My Brand', 'Main Competitor', 'Industry Trends', and 'Product Feedback'. Would you like to see the latest mentions for 'My Brand'?

---

**👤 You:**
> "Show me the sentiment breakdown for the 'Main Competitor' query."

**🤖 AI Agent:**
> The sentiment for 'Main Competitor' over the last 7 days is 15% Positive, 55% Neutral, and 30% Negative. Negative sentiment has increased by 5% compared to last week. Should I list the negative mentions?

---

**👤 You:**
> "What are the top media sources for 'Industry Trends'?"

**🤖 AI Agent:**
> The top 3 media sources for 'Industry Trends' are 'TechCrunch' (12 mentions), 'The Verge' (8 mentions), and 'Twitter' (45 posts). Would you like to see the most recent article from 'TechCrunch'?


## Installation & Usage

To install and use the **Determ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/determ](https://vinkius.com/mcp/determ)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

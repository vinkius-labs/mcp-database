# Influencers Club MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/influencers-club)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/influencers-club-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/influencers-club-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Discover and connect with influencers across social platforms with verified engagement data and audience demographics.

## Description
Connect your **Influencers Club** account to any AI agent and discover creators through natural conversation.

### What you can do

- **Creator Search** — Search influencers by niche, follower count, engagement rate, and platform
- **Profile Enrichment** — Enrich creator profiles by social handle or email address with full analytics
- **Similar Creators** — Find influencers similar to any given creator for campaign expansion
- **Audience Overlap** — Analyze audience overlap between two creators for partnership decisions
- **Content Analysis** — Browse recent posts from any creator with engagement metrics
- **Engagement Tracking** — View engagement rates, follower growth, and content performance

### How it works

1. Subscribe to this server
2. Enter your Influencers Club API Key
3. Start discovering creators from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — discover and vet influencers for brand campaigns
- **PR Agencies** — find creators by niche and analyze audience fit
- **Brand Managers** — evaluate partnerships through audience overlap analysis


## Available Tools
- **enrich_by_email**: Convert an email address into a full social profile
- **enrich_by_handle**: Get full profile data using a social media handle
- **get_audience_overlap**: Analyze shared audiences between different creators
- **get_creator_posts**: Access recent posts and historical content data
- **get_similar_creators**: Find lookalike profiles based on a specific creator
- **get_usage**: Monitor API consumption and usage limits
- **get_user_info**: Check account status and remaining credits
- **search_creators**: Search for creators using filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Influencers Club** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find tech influencers with 50K-500K followers and high engagement rates."

**🤖 AI Agent:**
> 12 tech influencers found (50K-500K, engagement >4%). Top 5: 1) @techsarah (285K followers, 6.2% engagement, AI/ML focus). 2) @codemaster (178K, 5.8%, Web Dev). 3) @devjames (142K, 7.1%, DevOps). 4) @airesearcher (98K, 8.4%, AI Research). 5) @startupguru (67K, 5.5%, Startups). Average engagement: 6.2% (industry avg: 2.8%). Would you like to enrich profiles or check audience overlap?

---

**👤 You:**
> "Enrich @techsarah's profile and find similar creators."

**🤖 AI Agent:**
> @techsarah profile: 285K followers (Instagram + YouTube). Engagement: 6.2%. Content: AI tutorials, tech reviews, conference talks. Audience: 65% male, 35% female. Age: 25-34 (52%). Location: US (45%), UK (15%), India (12%). Growth: +8.2K/month. Similar creators: 5 found. @airesearcher (98K, 8.4%, same AI niche). @mlpractitioner (120K, 5.1%). @techreviewer (210K, 4.8%). @codingwithjane (89K, 6.7%). @futuretech (156K, 5.3%). Would you like audience overlap analysis?

---

**👤 You:**
> "Analyze audience overlap between @techsarah and @airesearcher, and show their recent posts."

**🤖 AI Agent:**
> Audience overlap: @techsarah ↔ @airesearcher — 34% overlap. Shared audience: 28.4K followers. Unique to @techsarah: 188K. Unique to @airesearcher: 64K. Combined unique reach: 280K. Shared demographics: 25-34 tech professionals. Verdict: Complementary audiences, good for co-promotion. Recent posts @techsarah: 'GPT-5 First Impressions' (45K views, 8.2% eng). @airesearcher: 'Fine-tuning LLMs Guide' (12K views, 9.1% eng). Would you like to search more creators?


## Installation & Usage

To install and use the **Influencers Club** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/influencers-club](https://vinkius.com/mcp/influencers-club)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

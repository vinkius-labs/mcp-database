# BrandMentions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brandmentions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brandmentions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brandmentions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Monitor social listening and brand mentions via BrandMentions — track keywords, manage projects, and list influencers directly from any AI agent.

## Description
Connect your **BrandMentions** social listening account to any AI agent and orchestrate your brand monitoring workflows through natural conversation.

### What you can do

- **On-the-Spot Searches** — Trigger immediate web and social media searches for specific keywords and retrieve the results instantly.
- **Campaign Management** — List all your active tracking projects or create new ones to continuously monitor your brand or competitors.
- **Mention Auditing** — Retrieve detailed mentions and sentiment analysis for your ongoing projects.
- **Influencer Discovery** — List key influencers associated with your tracked keywords and projects.
- **Credit Tracking** — Check your API limits and remaining credits in real-time.

### How it works

1. Subscribe to this server
2. Enter your BrandMentions API Key
3. Start monitoring the web from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **PR & Marketing Teams** — quickly check recent mentions and brand sentiment without opening the main dashboard.
- **Brand Managers** — set up new tracking campaigns for product launches straight from their workflow tools.
- **Analysts** — retrieve structured mention data and influencer lists using natural language.


## Available Tools
- **add_project**: Create a new project for daily tracking
- **delete_project**: Delete a project
- **get_influencers**: List influencers for a specific project
- **get_mentions**: Get full results for a completed search job
- **get_processed_mentions**: Get partial results for a running search job
- **get_project_mentions**: Retrieve mentions for a specific project
- **get_remaining_credits**: Get current API credits limit/usage
- **list_projects**: List all active campaigns/projects
- **post_search**: Start an on-the-spot search job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrandMentions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tracking projects in BrandMentions."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active campaigns: 'Acme Corp Brand' (ID: proj_1), 'Competitor Analysis' (ID: proj_2), and 'Q3 Product Launch' (ID: proj_3).

---

**👤 You:**
> "Start a quick search for the keyword 'Vinkius'."

**🤖 AI Agent:**
> The search job has been started. The tracking hash is `hash_abc123`. You can query the results in a few moments.

---

**👤 You:**
> "Show me the top influencers for project proj_1."

**🤖 AI Agent:**
> Retrieving influencers... The top voices discussing your brand are TechReviewer (Score: 95) and MarketingGuru (Score: 88).


## Installation & Usage

To install and use the **BrandMentions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brandmentions](https://vinkius.com/mcp/brandmentions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

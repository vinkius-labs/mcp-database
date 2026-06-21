# Reddit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reddit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/reddit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/reddit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate Reddit interactions via AI — search subreddits, list hot posts, and retrieve comment threads directly.

## Description
Connect your **Reddit** account to any AI agent and take full control of your social discovery and community orchestration through natural conversation. Reddit is the 'front page of the internet', and this integration allows you to retrieve subreddit metadata, monitor trending posts, and analyze full comment threads directly from your chat interface.

### What you can do

- **Subreddit & Community Orchestration** — List hot, new, or top posts from any subreddit and retrieve detailed community metadata programmatically.
- **Search & Discovery Intelligence** — Perform global searches across all of Reddit to find relevant discussions and trending topics via natural language.
- **Conversation Deep-Dive** — Retrieve complete comment threads for specific posts to analyze community sentiment and synthesized insights directly from the AI interface.
- **User Profile Control** — Access and monitor public user profiles to understand community contributors and their engagement history.
- **Operational Monitoring** — Track system responses and manage rate limits to ensure your community analysis is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Reddit Client ID and Client Secret from your apps preferences
3. Start managing your social intelligence from Claude, Cursor, or any MCP-compatible client

No more manual scrolling or context switching. Your AI acts as a dedicated social analyst or community researcher.

### Who is this for?

- **Market Researchers** — quickly retrieve community feedback and monitor industry trends without switching apps.
- **Content Marketers** — automate the discovery of viral topics and track engagement across relevant subreddits via natural conversation.
- **Data Scientists** — streamline the retrieval of social metadata and monitor community discussions directly within the chat.


## Available Tools
- **get_post**: Get details for a specific Reddit post
- **get_subreddit_rules**: Get the rules of a subreddit
- **get_user_comments**: Get recent comments by a Reddit user
- **list_trending_subreddits**: List popular and trending subreddits
- **get_post_comments**: Get the comment thread for a post
- **get_subreddit_info**: Get metadata for a subreddit
- **get_user_profile**: Get details for a Reddit user
- **list_popular_posts**: List trending posts globally
- **list_subreddit_posts**: Supports sorting.

List posts from a subreddit
- **search_reddit**: Search all of Reddit
- **search_subreddit**: Search within a specific subreddit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reddit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the hot posts in r/artificialintelligence."

**🤖 AI Agent:**
> I've retrieved the hot posts. Currently, the top discussions are about 'New LLM Benchmarks' and 'AI in Robotics'. Would you like me to fetch the comments for any of them?

---

**👤 You:**
> "Show me the top trending posts in r/technology from the past 24 hours."

**🤖 AI Agent:**
> Top 5 in r/technology (24h). #1: "OpenAI announces GPT-5 with 10x context window" (23,400 upvotes, 4,567 comments). #2: "EU passes landmark AI regulation framework" (18,200 upvotes, 3,234 comments). #3: "Apple reveals M5 chip benchmarks" (15,800 upvotes, 2,100 comments). #4: "Quantum computing milestone: 1000 logical qubits" (12,400 upvotes, 1,890 comments). #5: "Tesla's new battery tech doubles EV range" (11,200 upvotes, 2,456 comments). Subreddit activity: 12% above average today.

---

**👤 You:**
> "Search r/startups for posts mentioning Series A funding advice from the last month."

**🤖 AI Agent:**
> Found 23 relevant posts in r/startups about Series A advice. Most upvoted: "What I wish I knew before our Series A" (2,340 upvotes, detailed founder retrospective). "Series A pitch deck template that raised $12M" (1,890 upvotes, includes template link). "VC red flags during Series A due diligence" (1,456 upvotes). Key themes: unit economics (mentioned 34 times), team composition (28), market timing (22), board structure (18). 3 AMA posts from Series A founders this month.


## Installation & Usage

To install and use the **Reddit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reddit](https://vinkius.com/mcp/reddit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

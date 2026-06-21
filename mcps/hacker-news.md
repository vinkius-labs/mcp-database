# Hacker News MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hacker-news)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hacker-news-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hacker-news-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Explore tech news via Hacker News — fetch top and new stories, retrieve detailed item contents, and read comments directly from any AI agent.

## Description
Connect to **Hacker News** (Y Combinator) and take full control of your tech news consumption, discussion auditing, and trend tracking through natural conversation.

### What you can do

- **Front Page Orchestration** — Fetch current Top stories to retrieve popular social links, titles, scores, and author metadata natively within your chat
- **Real-time Submission Tracking** — Iterate through chronological submissions to discover cutting-edge tech updates and new project launches flawlessly
- **Detailed Item Auditing** — Read the full contents of specific HN items (stories, comments, or polls) by their numeric IDs to extract exact textual context
- **Clean Comment Retrieval** — Retrieve discussion threads with HTML comments converted cleanly into Markdown, allowing your AI agent to reason with structured conversations limitlessly
- **Story Metadata Inspection** — Analyze specific node blocks identifying submission times, URL references, and total comment counts synchronously
- **Trend Discovery** — Identify high-ranking tech discussions and gather required IDs to browse and discover ongoing community debates natively

### How it works

1. Subscribe to this server
2. No authentication required (Public API)
3. Start exploring tech news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers & Engineers** — stay updated on the latest tech trends and library releases without manual browsing
- **Product Managers** — monitor community feedback and discover new product launches using natural language conversation
- **Researchers** — audit discussion threads and extract key insights from tech-focused community debates in real-time
- **Curious Professionals** — quickly summarize top stories and read insightful comments through the chat interface


## Available Tools
- **top_stories**: Fetch the current Top stories on the Hacker News front page
- **new_stories**: Fetch the most recently submitted stories on Hacker News
- **get_item**: Read the detailed contents of a specific Hacker News item (a story, comment, or poll) by its ID. Returns HTML comments converted cleanly to Markdown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hacker News** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 stories on Hacker News right now"

**🤖 AI Agent:**
> Retrieving top stories... I found 5 trending items including 'Release of New AI Protocol' (Score: 450) and 'Advancements in Fusion Energy'. Would you like the link or comments for any of these?

---

**👤 You:**
> "Get details and comments for HN item 123456"

**🤖 AI Agent:**
> Retrieving item 123456... Title: 'Mastering Rust for Systems Programming'. I've also fetched 10 top-level comments discussing memory safety and performance. Would you like me to summarize the discussion?

---

**👤 You:**
> "What are the newest submissions on tech launches?"

**🤖 AI Agent:**
> Checking newest stories... I found several recent submissions including 'Show HN: A new open-source database' and 'Beta release of WebFramework X'. I can provide the IDs if you want to track their progress.


## Installation & Usage

To install and use the **Hacker News** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hacker-news](https://vinkius.com/mcp/hacker-news)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

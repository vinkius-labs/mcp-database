# Hacker News MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hacker-news-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hacker-news-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hacker-news-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Hacker News stories, comments, and user profiles directly from your AI agent to stay updated on the latest tech trends.

## Description
Connect to the **Hacker News** API to browse the pulse of the developer community directly through your AI agent.

### What you can do

- **Story Feeds** — Retrieve the latest, top, and best stories, including specialized feeds like 'Ask HN', 'Show HN', and Job postings.
- **Item Inspection** — Fetch deep details for any specific story, comment, or poll using its unique integer ID.
- **User Profiles** — Analyze user karma, submission history, and profile metadata for any public username.
- **Real-time Updates** — Monitor the latest item and profile changes across the platform to see what is trending right now.
- **Discovery** — Use the max item tool to walk through the history of the site or find the newest content as it is indexed.

### How it works

1. Subscribe to this server
2. No API key is required for the public Hacker News API
3. Start querying tech news from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — stay updated on libraries, frameworks, and industry shifts without leaving the terminal or IDE
- **Researchers** — analyze community sentiment and trending topics in the tech ecosystem
- **Tech Enthusiasts** — never miss a viral post or a significant 'Show HN' launch


## Available Tools
- **get_ask_stories**: Get up to 200 latest Ask HN stories
- **get_best_stories**: Get up to 500 best stories
- **get_item**: Get details for a specific Hacker News item
- **get_job_stories**: Get up to 200 latest Job stories
- **get_max_item**: Get the current largest item ID
- **get_new_stories**: Get up to 500 new stories
- **get_show_stories**: Get up to 200 latest Show HN stories
- **get_top_stories**: Get up to 500 top stories
- **get_updates**: Get item and profile changes
- **get_user**: Get details for a specific Hacker News user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hacker News** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the top 5 stories on Hacker News right now?"

**🤖 AI Agent:**
> I'll fetch the top stories for you. Using `get_top_stories`, I've found the current leaders: 1. 'New LLM release' (ID: 123), 2. 'Open Source Database' (ID: 124)... Would you like details on any of these?

---

**👤 You:**
> "Get the profile details and karma for user 'pg'."

**🤖 AI Agent:**
> Fetching profile for 'pg' via `get_user`... Paul Graham has 156,000 karma and has been a member since 2006. He has submitted over 10,000 items. Would you like to see his recent submissions?

---

**👤 You:**
> "Tell me more about the story with ID 42301234."

**🤖 AI Agent:**
> Inspecting item 42301234 using `get_item`... This is a story titled 'The Future of MCP' by user 'techie'. It has 450 points and 82 comments. The URL points to a GitHub repository. Should I summarize the comments for you?


## Installation & Usage

To install and use the **Hacker News** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hacker-news-alternative](https://vinkius.com/mcp/hacker-news-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

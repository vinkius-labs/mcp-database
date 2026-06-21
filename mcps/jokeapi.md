# JokeAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jokeapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jokeapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jokeapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Universal humor engine — get random jokes, filter by category and safety flags via AI.

## Description
Equip your AI agent with a source of laughter via the **JokeAPI** MCP server. This integration provides access to a large database of jokes across various categories like Programming, Pun, and Misc. Your agent can retrieve random jokes, filter them by specific categories or languages, and ensure content safety using blacklist flags (nsfw, religious, political, etc.). Whether you're building a fun bot, looking for a quick icebreaker, or just want a laugh, your agent acts as a dedicated comedian through natural conversation.

### What you can do

- **Random Jokes** — Get a single random joke or a list of multiple jokes.
- **Category Filtering** — Choose from Programming, Misc, Pun, Spooky, or Christmas categories.
- **Content Safety** — Use flags to filter out jokes that are NSFW, religious, political, or offensive.
- **Language Support** — Access jokes in multiple languages including English, German, and Portuguese.
- **Humor Auditing** — Summarize multiple jokes to identify popular themes and comedic structures.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start getting jokes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Entertainment Apps** — add a humor feature to your AI-driven applications.
- **Bot Developers** — build engaging and fun chat bots with varied content.
- **General Users** — enjoy a quick laugh or find jokes to share with friends.
- **Social Media Managers** — source lighthearted content for audience engagement.


## Available Tools
- **list_joke_categories**: List joke categories
- **get_joke**: Get a random joke
- **list_jokes**: Get multiple jokes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JokeAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me a programming joke."

**🤖 AI Agent:**
> Sure! Why do programmers always mix up Halloween and Christmas? Because Oct 31 equals Dec 25! Want to hear another one?

---

**👤 You:**
> "Give me 3 safe jokes from the 'Misc' category."

**🤖 AI Agent:**
> Retrieving 3 safe miscellaneous jokes... Here is the first one: 'I'm reading a book on anti-gravity. It's impossible to put down!' Ready for the others?

---

**👤 You:**
> "Do you have any 'Spooky' jokes for Halloween?"

**🤖 AI Agent:**
> Fetching a spooky joke... 'Why don't ghosts like rain? Because it damps their spirits!' I can find more themed jokes if you're planning a party.


## Installation & Usage

To install and use the **JokeAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jokeapi](https://vinkius.com/mcp/jokeapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# SaveDay MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/saveday)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/saveday-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/saveday-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Capture, organize, and summarize content from URLs, text, and images directly into your SaveDay knowledge base.

## Description
Connect your **SaveDay** account to any AI agent to seamlessly capture and retrieve information. SaveDay acts as your second brain, allowing you to store web content, notes, and images, and then query them using natural language.

### What you can do

- **Content Capture** — Instantly save URLs, text snippets, or images with custom titles and tags using the `capture_content` tool.
- **Smart Search** — Query your saved items using natural language with `search_items` to find exactly what you need without manual sorting.
- **AI Summarization** — Use `get_summary` to generate concise summaries of your saved content to grasp key points quickly.
- **Tag Management** — List and organize your knowledge base using the `list_tags` tool for better categorization.

### How it works

1. Subscribe to this server
2. Enter your SaveDay API Key
3. Start capturing and searching your knowledge base from Claude, Cursor, or any MCP-compatible client.


## Available Tools
- **capture_content**: Type must be url, text, or image.

Capture a URL, text, or image to SaveDay
- **search_items**: Search through saved items
- **get_summary**: Retrieve an AI-generated summary for a specific saved item
- **list_tags**: Retrieve a list of all tags used in the SaveDay account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SaveDay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Save this URL to my SaveDay with the tag 'research': https://example.com/ai-mcp"

**🤖 AI Agent:**
> I've successfully captured the content from the URL. It has been saved to your SaveDay account with the tag 'research'.

---

**👤 You:**
> "Search my SaveDay for any notes about 'smart home automation'."

**🤖 AI Agent:**
> I found 3 items related to 'smart home automation'. Would you like me to summarize the most recent one or list them all?

---

**👤 You:**
> "Show me all the tags I have used in SaveDay."

**🤖 AI Agent:**
> Here are your current tags: 'research', 'work', 'recipes', 'travel', and 'ai-tools'.


## Installation & Usage

To install and use the **SaveDay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saveday](https://vinkius.com/mcp/saveday)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Poe MCP Server

Manage AI chatbots on Poe — create bots, query other AI models, monitor messages, and track usage stats.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/poe)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Connect your **Poe** (Quora's AI platform) account to any AI agent and manage your chatbot empire through natural conversation. Create bots, chain AI model responses, monitor conversations, and track performance — all via API.

### What you can do
- **Bot Management** — List, create, update, and delete API bots programmatically
- **AI Model Chaining** — Query any bot on Poe (GPT-4, Claude, etc.) from your bot using API v2
- **Message Monitoring** — View recent conversations, debug responses, and analyze user interactions
- **Usage Statistics** — Track message counts, unique users, response times, and error rates
- **Endpoint Testing** — Send test messages to verify bot connectivity and response quality
- **Multi-Model Workflows** — Build complex bots that combine responses from multiple AI models

### How it works
1. Subscribe to this server
2. Enter your Poe API access token from creator.poe.com
3. Start managing bots from Claude, Cursor, or any MCP client

### Who is this for?
- **Bot Developers** — Create and manage AI bots without leaving your code editor
- **AI Researchers** — Chain multiple AI models and compare responses programmatically
- **Community Managers** — Monitor bot conversations and track engagement metrics


## Available Tools
- **create_bot**: Requires a bot name, base URL for your API endpoint, and the model name. Optionally set a system prompt and description.

Create a new API bot on Poe
- **delete_bot**: This action cannot be undone. All conversation history and settings for the bot will be lost.

Delete a Poe API bot
- **list_available_bots**: Useful for discovering which AI models and specialized bots are available for chaining in your bot workflows.

List publicly available bots on Poe that your bot can query
- **get_bot_stats**: Essential for monitoring bot health, understanding user engagement, and identifying performance bottlenecks.

Get usage statistics for a Poe bot
- **get_bot**: Use the bot ID obtained from list_bots.

Get details of a specific Poe bot
- **list_bots**: Returns bot names, handles, models, and status. Essential first step to identify which bot to work with before querying, updating, or checking stats.

List all API bots under your Poe account
- **list_messages**: Useful for monitoring what users are asking, debugging bot responses, and analyzing conversation patterns. Returns message content, timestamps, and user identifiers.

List recent messages for a specific Poe bot
- **query_bot**: This allows chaining bot responses - your bot can query GPT-4, Claude, or any other bot on Poe and use the response as input. The cost is covered by the user's free message limit or subscription.

Query another bot on Poe from your bot
- **send_message**: Useful for testing endpoint connectivity and validating bot responses. The bot will process the message and return a response via its configured endpoint.

Send a message to a Poe bot (simulate user interaction)
- **update_bot**: Changes take effect immediately for new conversations.

Update an existing Poe bot's configuration


## Installation & Usage

To install and use the **Poe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poe](https://vinkius.com/mcp/poe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

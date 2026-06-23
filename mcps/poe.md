# Poe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/poe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage AI chatbots on Poe — create bots, query other AI models, monitor messages, and track usage stats.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bots and show stats for the first one."

**🤖 AI Agent:**
> 🤖 You have 3 bots: SummaryBot, Translator, CodeAssistant. Stats for SummaryBot: 1,247 messages, 89 unique users, avg response 2.3s.

---

**👤 You:**
> "Create a bot called 'Research Assistant' using GPT-4 that summarizes articles."

**🤖 AI Agent:**
> ✅ Bot created! 'Research Assistant' (ID: bot_123) using GPT-4. Configure your endpoint URL in the bot settings.

---

**👤 You:**
> "Query Claude-3.5-Sonnet from my ResearchBot: 'What are the key trends in AI?'"

**🤖 AI Agent:**
> 🤖 Claude-3.5-Sonnet responded: 'Key AI trends include multimodal models, agentic workflows, and reasoning capabilities...' Response received successfully.


## ❓ FAQ

**Q: How do I get a Poe API access token?**
Go to [creator.poe.com](https://creator.poe.com/), navigate to Settings > API, and generate an access token. This token authenticates all API requests for bot management.

**Q: What AI models can I query through Poe?**
Poe has GPT-4, GPT-4o, Claude 3.5 Sonnet, Claude 3 Opus, Llama 3, and dozens of specialized bots. Use query_bot to chain responses from multiple models in your workflows.

**Q: How does bot chaining work?**
Using Poe API v2, your bot can query any other bot on Poe for free. The response becomes input for your bot's processing. Costs are covered by the user's free message limit or subscription.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poe](https://vinkius.com/mcp/poe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Poe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Poe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poe": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

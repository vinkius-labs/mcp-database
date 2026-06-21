# Perplexity AI MCP Server

Access Perplexity's AI search and chat models — get web-grounded answers with citations, search the web and run AI conversations from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/perplexity-ai-alternative)

## Overview
**Category:** ai-frontier
**Tools Count:** 8

## Description
Connect your **Perplexity AI** account to any AI agent and leverage web-grounded AI models through natural conversation.

### What you can do

- **Chat Completions** — Send conversations to Perplexity models (sonar, sonar-pro, sonar-reasoning) and receive responses with web citations
- **Web Search** — Search the web using Perplexity's dedicated Search API with domain filtering
- **Sonar API** — Get web-grounded responses from the Sonar model with citations and source URLs
- **Model Discovery** — List all available Perplexity models and their capabilities

### How it works

1. Subscribe to this server
2. Enter your Perplexity API Key
3. Start using Perplexity models from Claude, Cursor, or any MCP-compatible client

No more switching between search engines and chat tools. Your AI acts as a web-grounded research assistant.

### Who is this for?

- **Researchers** — get web-grounded answers with citations for fact-checking and literature review
- **Developers** — integrate web search and AI chat into applications via API
- **Analysts** — search the web with domain filters and get structured search results


## Available Tools
- **chat**: Requires the model ID (e.g. "sonar", "sonar-pro", "sonar-reasoning") and messages array in JSON format. Each message must have a "role" ("user", "assistant" or "system") and "content" (text). Optionally set max_tokens, temperature (0-1), top_p (0-1), search domain filter, and whether to return images or related questions. Returns the assistant's response with citations.

Send a chat message to a Perplexity model
- **chat_pro**: Requires messages array in JSON format. Optionally set max_tokens and temperature. Returns the assistant's response with citations.

Send a chat message to the Sonar Pro model for enhanced responses
- **chat_with_reasoning**: Requires messages array in JSON format. Optionally set max_tokens, temperature and reasoning_effort (low, medium, high). Returns the assistant's response with detailed reasoning chain.

Send a message to the Sonar Reasoning model for step-by-step reasoning
- **chat_with_reasoning_pro**: Requires messages array in JSON format. Optionally set max_tokens, temperature and reasoning_effort (low, medium, high). Returns the assistant's response with detailed reasoning chain and citations.

Send a message to the Sonar Reasoning Pro model for deep reasoning
- **get_usage**: Useful for monitoring API consumption and staying within usage limits.

Get API usage statistics
- **list_models**: Each model returns its ID (e.g. "sonar", "sonar-pro", "sonar-reasoning", "sonar-reasoning-pro"), display name and capabilities. Use this to discover which models are available and their IDs for use with the chat and sonar tools.

List all available Perplexity models
- **search**: Returns search results with snippets, citations and source URLs. Requires the search query. Optionally set max_results and domain filter to limit results to specific websites.

Search the web using Perplexity Search API
- **sonar**: This is the core search-enhanced model. Requires messages array in JSON format. Optionally set max_tokens and temperature. Returns the assistant's response with web citations.

Send a message to the Sonar model for web-grounded responses


## Installation & Usage

To install and use the **Perplexity AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/perplexity-ai-alternative](https://vinkius.com/mcp/perplexity-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

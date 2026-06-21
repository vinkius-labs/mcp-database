# Eden AI MCP Server

Access 100+ AI models through a single API — route LLMs, generate embeddings, and execute specialized AI tasks like OCR and translation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/eden-ai-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 13

## Description
Connect **Eden AI** to your AI agent and unlock the power of over 100 leading AI providers through a single, unified interface. Orchestrate models from OpenAI, Google, Anthropic, and more without managing multiple API keys.

### What you can do

- **LLM Routing** — Use `chat_completions` with smart routing (@edenai) or specify specific provider/model combinations for conversational tasks.
- **Specialized AI Experts** — Execute synchronous or asynchronous tasks like OCR, Translation, Image Generation, and Speech-to-Text using `universal_ai_sync` and `universal_ai_async`.
- **Embeddings & Search** — Convert text into numerical vectors with `create_embedding` and explore available models via `list_embedding_models`.
- **File Management** — Upload, list, and delete files in Eden AI's persistent storage to provide context for specialized AI features.
- **Usage Monitoring** — Keep track of your consumption and available balance with `check_credits`.

### How it works

1. Subscribe to this server
2. Enter your Eden AI API Key
3. Start querying dozens of AI providers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — quickly test and compare different models (GPT-4, Claude 3, Gemini) without rewriting integration code
- **Automation Engineers** — build complex workflows involving OCR, translation, and audio processing using a single API standard
- **Data Scientists** — generate embeddings across various providers to find the best fit for RAG or semantic search applications


## Available Tools
- **check_credits**: Check current Eden AI credit balance
- **list_files**: List all files uploaded to Eden AI
- **chat_completions**: Use @edenai for smart routing or specify provider/model.

Create a chat completion using Eden AI LLM routing
- **create_custom_token**: Create a custom API token with specific constraints
- **create_embedding**: Convert text into numerical vectors
- **create_stateful_response**: Create a stateful chat response that stores history server-side
- **delete_files**: Delete files from Eden AI storage
- **get_async_job**: Get the status and results of an asynchronous Universal AI job
- **list_embedding_models**: List available embedding models
- **monitor_consumption**: Monitor API consumption and costs
- **universal_ai_async**: Start an asynchronous expert model job (e.g., Speech-to-Text)
- **universal_ai_sync**: Model format: feature/subfeature/provider[/model]

Execute synchronous expert models (OCR, Translation, Image Gen)
- **upload_file**: Upload a file to Eden AI persistent storage


## Installation & Usage

To install and use the **Eden AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eden-ai-alternative](https://vinkius.com/mcp/eden-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

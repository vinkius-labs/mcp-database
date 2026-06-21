# Mistral AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mistral-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mistral-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mistral-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access Mistral AI models via API — chat with Claude alternatives, generate embeddings, moderate content and manage batch jobs from any AI agent.

## Description
Connect your **Mistral AI** account to any AI agent and leverage European-built AI models through natural conversation.

### What you can do

- **Model Discovery** — List all available Mistral models with their IDs, capabilities and context windows
- **Chat Completions** — Send conversations to Mistral models (large, small, codestral, nemo) and receive responses with configurable parameters
- **Embeddings** — Generate vector embeddings for semantic search, similarity comparison and vector storage
- **Content Moderation** — Check text for harmful categories (violence, hate, sexual, self-harm) with safety scores
- **File Management** — List and delete uploaded files used for batch processing and document AI
- **Batch Processing** — Create, track and cancel batch jobs for cost-effective asynchronous processing

### How it works

1. Subscribe to this server
2. Enter your Mistral AI API Key
3. Start using Mistral models from Claude, Cursor, or any MCP-compatible client

No more switching between API tools to interact with Mistral. Your AI acts as an LLM orchestration layer.

### Who is this for?

- **Developers** — quickly send messages to Mistral models, generate embeddings and moderate content without writing HTTP code
- **ML Engineers** — discover available models, compare capabilities and batch-process many prompts efficiently
- **Content Teams** — review model outputs, moderate user-generated content and manage batch processing jobs via conversation


## Available Tools
- **cancel_batch**: Provide the batch ID. This is useful if you submitted a large batch by mistake and want to stop further processing.

Cancel a running batch job
- **chat**: Requires the model ID (e.g. "mistral-large-latest", "mistral-small-latest", "codestral-latest") and messages array in JSON format. Each message must have a "role" ("user", "assistant" or "system") and "content" (text). Optionally set max_tokens, temperature (0-1), top_p (0-1) and tools array for function calling. Returns the assistant's response.

Send a chat message to a Mistral model
- **create_batch**: Requires the input file ID (containing JSONL requests) and the endpoint (e.g. "/v1/chat/completions"). Returns the batch with its ID for tracking. Use list_batches and get_batch to monitor progress.

Create a batch processing job
- **delete_file**: Provide the file ID from list_files. WARNING: this action is irreversible.

Delete an uploaded file from Mistral
- **embeddings**: Requires the model ID and text input (string or array of strings). Returns embedding vectors for each input text. Useful for semantic search, similarity comparison and vector database storage.

Generate embeddings using Mistral
- **get_batch**: Provide the batch ID.

Get details for a specific batch job
- **list_batches**: Each batch shows its ID, status (queued, running, succeeded, failed, cancelled), input/output file IDs and request counts.

List batch processing jobs
- **list_files**: Files are used for fine-tuning, batch processing and document AI. Each file shows its ID, filename, purpose, size and upload date.

List files uploaded to Mistral
- **list_models**: Each model returns its ID (e.g. "mistral-large-latest", "mistral-small-latest", "codestral-latest"), display name, capabilities and context window. Use this to discover which models are available and their IDs for use with the chat tool.

List all available Mistral AI models
- **moderate**: ). Requires the input text (string or array). Returns safety scores for each category. Useful for content filtering and safety checks before processing user input.

Moderate text content with Mistral


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mistral AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to Mistral Large asking 'What is the capital of France?'"

**🤖 AI Agent:**
> Mistral responded: 'The capital of France is Paris. It is the most populous city in France and serves as the country's political, economic, and cultural center.'

---

**👤 You:**
> "List all available Mistral models."

**🤖 AI Agent:**
> Available models: mistral-large-latest (most capable, 128K context), mistral-small-latest (efficient, 32K context), codestral-latest (code specialist, 32K context), mistral-embed (embeddings, 8K context).

---

**👤 You:**
> "Moderate this text: 'I want to learn about AI safety and content filtering.'"

**🤖 AI Agent:**
> The text passed moderation with all safety scores below thresholds. Categories checked: sexual (0.01), hate (0.00), violence (0.00), self-harm (0.00), criminal (0.00). Content is safe to process.


## Installation & Usage

To install and use the **Mistral AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mistral-ai](https://vinkius.com/mcp/mistral-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

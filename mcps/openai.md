# OpenAI MCP Server

Use GPT-4o, DALL-E 3, embeddings, fine-tuning, and moderation as tools inside your AI agent workflows.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openai)

## Overview
**Category:** superpower
**Tools Count:** 10

## Description
Connect the **OpenAI** API to any AI agent and unlock the full power of GPT models as composable tools.

### What you can do

- **Chat Completions** — Generate responses from GPT-4o, GPT-4o-mini, and other models
- **Image Generation** — Create images with DALL-E 3 from text descriptions
- **Embeddings** — Convert text to vector representations for semantic search
- **Content Moderation** — Check text for policy violations automatically
- **Fine-tuning** — Create and monitor custom model training jobs
- **File Management** — List uploaded files for training and assistants
- **Assistants** — Browse configured OpenAI Assistants
- **Structured Output** — Generate structured JSON responses from prompts


## Available Tools
- **create_fine_tune**: Requires a previously uploaded JSONL training file ID.

Create a fine-tuning job
- **list_fine_tunes**: List fine-tuning jobs
- **chat_completion**: Specify model (gpt-4o, gpt-4o-mini, etc.) and messages array as JSON.

Generate a chat completion using OpenAI models
- **structured_output**: Provide a system prompt and user message.

Generate structured JSON output from a prompt
- **list_models**: List available OpenAI models
- **create_embedding**: Create text embeddings
- **generate_image**: Returns the image URL.

Generate an image with DALL-E 3
- **list_files**: List uploaded files
- **moderate_content**: Check content for policy violations
- **list_assistants**: List OpenAI Assistants


## Installation & Usage

To install and use the **OpenAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openai](https://vinkius.com/mcp/openai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

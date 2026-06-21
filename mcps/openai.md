# OpenAI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Use GPT-4o, DALL-E 3, embeddings, fine-tuning, and moderation as tools inside your AI agent workflows.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask GPT-4o to summarize this document in 3 bullet points."

**🤖 AI Agent:**
> Here's the GPT-4o summary:

• **Revenue grew 23%** YoY driven by enterprise contracts
• **Operating costs decreased** 8% through automation initiatives
• **Customer retention** reached 94%, highest in company history

---

**👤 You:**
> "Generate an image of a futuristic cityscape at sunset."

**🤖 AI Agent:**
> 🎨 Image generated!

- **URL**: https://oaidalleapiprodscus.blob.core.windows.net/...
- **Size**: 1024x1024
- **Revised prompt**: A breathtaking futuristic cityscape...

---

**👤 You:**
> "Check if this text violates content policies."

**🤖 AI Agent:**
> ✅ Content analysis complete:

| Category | Flagged | Score |
|----------|---------|-------|
| Hate | No | 0.001 |
| Violence | No | 0.002 |
| Sexual | No | 0.000 |
| Self-harm | No | 0.000 |

No policy violations detected.


## Installation & Usage

To install and use the **OpenAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openai](https://vinkius.com/mcp/openai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Together AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/together-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/together-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/together-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate code, evaluate embeddings, and deploy open-source LLMs instantly from your local agent via Together AI's infrastructure.

## Description
Connect your **Together AI** account to any AI agent and integrate bleeding-edge open-source models seamlessly into your workflow. Harness world-class inference speeds to query Llama, Mixtral, and more, or orchestrate specialized model fine-tuning jobs straight from your chat environment.

### What you can do

- **Model Discovery** — Explore and list all currently supported models on the Together network, identifying the best engine for any NLP or vision task
- **Conversational AI** — Run chat completion cycles on advanced models simply by supplying a model ID directly from the chat prompt
- **Vector Storage Preparation** — Generate instant rich embeddings for input texts, ready to populate your analytical databases
- **Creative Media** — Instruct external diffusion models to generate images using detailed physical descriptions
- **Custom Fine-Tuning** — Provision custom training runs by indicating a base framework and dataset file, alongside tracking existing job statuses

### How it works

1. Sign up for this integration
2. Open your api.together.xyz control panel and fetch a developer API Key
3. Plug the key above, specify models to your agent, and enjoy sub-second serverless inference directly inside your command interface

### Who is this for?

- **AI Developers** — Orchestrate fine-tuning parameters and launch jobs to the compute cluster without CLI switching
- **Software Engineers** — Use the provider to test completions using alternative open-source solutions (e.g., Llama 3) natively in code editors
- **Machine Learning Engineers** — Bulk-generate vectors from raw logs using embedding models attached straight to their main conversational agent


## Available Tools
- **chat_completion**: Provide a model ID and a JSON array of messages.

Executes a chat completion using Together AI models
- **text_completion**: Provide a model ID and a prompt.

Executes a base text completion
- **create_finetune_job**: Provide a base model ID and a training file ID.

Creates a new fine-tuning job
- **generate_embeddings**: Provide a model ID and a JSON array of strings.

Generates vector embeddings for input texts
- **generate_image**: Provide a model ID and descriptive prompt.

Generates an image from a text prompt
- **list_finetune_jobs**: Lists all fine-tuning jobs
- **list_available_models**: Lists all AI models available on Together AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Together AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the models currently available on Together AI."

**🤖 AI Agent:**
> I've fetched 132 available models. Here are the top chat models:
- meta-llama/Llama-2-70b-chat-hf
- mistralai/Mixtral-8x7B-Instruct-v0.1
- google/gemma-7b-it
Ask if you want the embedding or image models only.

---

**👤 You:**
> "Generate an embedding array using model `togethercomputer/m2-bert-80M-8k-retrieval` for the sentence 'The cat sat on the mat'."

**🤖 AI Agent:**
> Embeddings generated successfully. Dimensions: 768. Sample values:
[-0.0124, 0.0411, 0.0812, ... -0.0123]


## Installation & Usage

To install and use the **Together AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/together-ai](https://vinkius.com/mcp/together-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

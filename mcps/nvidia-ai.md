# NVIDIA AI MCP Server

Access LLMs, embeddings, code generation, and reasoning via NVIDIA API Catalog.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nvidia-ai)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect **NVIDIA AI** to any AI agent and harness the power of GPU-accelerated foundation models — chat with Llama, generate embeddings, write code with CodeLlama, translate text, and perform complex reasoning through the NVIDIA API Catalog.

### What you can do
- **Chat with LLMs** — Access Llama 3.1, Mistral, Nemotron, and more via chat completions
- **Generate Embeddings** — Create vector embeddings for search and clustering
- **Code Generation** — Write code from natural language prompts using CodeLlama
- **Summarization** — Condense long documents into concise summaries
- **Translation** — Neural translation between dozens of languages
- **Text-to-SQL** — Convert natural language questions into SQL queries
- **Sentiment Analysis** — Analyze the emotional tone of text
- **Complex Reasoning** — Ask questions to the 405B-parameter reasoning model

### How it works
1. Subscribe to this server
2. Enter your NVIDIA API Key (from build.nvidia.com)
3. Start running AI models from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Developers** — Prototype AI features without managing GPU infrastructure
- **Data Scientists** — Generate embeddings and run NLP tasks at scale
- **Business Analysts** — Use text-to-SQL to query databases with natural language


## Available Tools
- **ask_question**: Optionally provide context for better answers.

Ask a question to a powerful reasoning model (405B params)
- **chat_completion**: Use "model" to specify which AI model (e.g., "meta/llama-3.1-70b-instruct", "mistralai/mistral-large"). Messages should be in OpenAI format: [{role: "user", content: "..."}].

Chat with an NVIDIA AI model (Llama, Mistral, etc)
- **generate_code**: Specify language if needed.

Generate code from a natural language prompt
- **get_embeddings**: Model: "nvidia/nv-embed-v1".

Generate vector embeddings from text
- **list_models**: List all available AI models on the NVIDIA API Catalog
- **text_to_sql**: Convert natural language to SQL query
- **analyze_sentiment**: Analyze the sentiment of a text
- **summarize_text**: Summarize long text into a concise version
- **translate_text**: Translate text to another language


## Installation & Usage

To install and use the **NVIDIA AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nvidia-ai](https://vinkius.com/mcp/nvidia-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

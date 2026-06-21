# Open WebUI MCP Server

Manage your Open WebUI instance — list models, handle chat completions, and manage RAG collections directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/open-webui)

## Overview
**Category:** loved-by-devs
**Tools Count:** 12

## Description
Connect your **Open WebUI** instance to any AI agent and take full control of your local and cloud LLM orchestration through natural conversation.

### What you can do

- **Model Management** — Use `list_models` to fetch all available models including Ollama, OpenAI, and Open WebUI Functions.
- **RAG & Knowledge Base** — Upload files with `upload_file`, process web content via `process_web_url`, and organize them into collections using `add_file_to_collection`.
- **Chat Orchestration** — Create and manage backend-controlled chats with `create_new_chat` or use OpenAI/Anthropic compatible endpoints like `chat_completions` and `send_message`.
- **Native Ollama Support** — Directly interact with the Ollama API using `ollama_generate`, `ollama_tags`, and `ollama_embed` for local inference tasks.
- **File Processing** — Monitor the status of your document ingestion with `get_file_status` to ensure your RAG context is ready.

### How it works

1. Subscribe to this server
2. Enter your Open WebUI Base URL and API Key
3. Start managing your LLM infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — automate the testing of different models and RAG configurations without leaving the terminal or IDE.
- **Knowledge Managers** — quickly ingest documentation and web URLs into Open WebUI collections via simple commands.
- **DevOps Teams** — monitor local Ollama instances and manage model availability across the organization.


## Available Tools
- **add_file_to_collection**: Add a file to a knowledge collection
- **chat_completed**: Run outlet filters for completed chat
- **chat_completions**: OpenAI-compatible chat completion
- **create_new_chat**: Must generate UUIDs for message IDs.

Create a new chat (Backend-Controlled Flow)
- **get_file_status**: Check file processing status
- **list_models**: Retrieve all models
- **ollama_embed**: Ollama API Embeddings
- **ollama_generate**: Ollama API Generate Completion
- **ollama_tags**: List Ollama models
- **process_web_url**: Process a web URL into a collection
- **send_message**: Anthropic-compatible message generation
- **upload_file**: Content is extracted and stored in the vector DB. Provide file content as base64.

Upload a file for RAG


## Installation & Usage

To install and use the **Open WebUI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-webui](https://vinkius.com/mcp/open-webui)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

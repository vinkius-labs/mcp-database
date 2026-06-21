# Open WebUI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-webui)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-webui-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-webui-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your Open WebUI instance — list models, handle chat completions, and manage RAG collections directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open WebUI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all models available in my Open WebUI instance."

**🤖 AI Agent:**
> I've retrieved the models. You have access to 'llama3:latest', 'gpt-4o', and several custom Open WebUI functions. Would you like to use one of them for a chat completion?

---

**👤 You:**
> "Process the URL 'https://docs.openwebui.com/' into my 'Documentation' collection."

**🤖 AI Agent:**
> I have started processing the URL. The content is being scraped and indexed into the 'Documentation' collection. You can now ask questions based on this data.

---

**👤 You:**
> "Generate a response using the 'llama3' model for the prompt 'Explain quantum computing'."

**🤖 AI Agent:**
> Using the `ollama_generate` tool with 'llama3': Quantum computing is a type of computing that uses quantum-mechanical phenomena... Would you like more details?


## Installation & Usage

To install and use the **Open WebUI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-webui](https://vinkius.com/mcp/open-webui)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

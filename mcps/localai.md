# LocalAI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/localai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/localai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/localai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Run LLMs, generate images, and process audio locally. OpenAI-compatible API for your own hardware.

## Description
Connect your **LocalAI** instance to any AI agent and leverage powerful multimodal capabilities directly from your own infrastructure.

### What you can do

- **Text Generation** — Use `chat_completions` or `anthropic_messages` to generate text using local models with full OpenAI or Anthropic compatibility.
- **Image Synthesis** — Create visual content from text prompts using the `generate_image` tool, supporting custom sizes and negative prompts.
- **Audio Processing** — Convert speech to text with `transcribe_audio` or generate natural-sounding speech from text using `text_to_speech`.
- **Advanced Search & RAG** — Generate vector embeddings with `create_embeddings` and improve search relevance using the `rerank_documents` tool.
- **Computer Vision** — Analyze images and identify elements using the `detect_objects` tool.
- **System Management** — Monitor your instance with `list_models`, `get_system`, and `getVersion` to ensure optimal performance.

### How it works

1. Subscribe to this server
2. Provide your LocalAI Base URL (e.g., `http://localhost:8080`) and optional API Key
3. Start interacting with your local models through Claude, Cursor, or any MCP client

### Who is this for?

- **Privacy-Conscious Developers** — Run powerful AI workflows without sending sensitive data to third-party cloud providers.
- **AI Researchers** — Easily test and swap different local models for chat, vision, and audio tasks.
- **DevOps Engineers** — Integrate local AI capabilities into internal tools and automated pipelines.


## Available Tools
- **anthropic_messages**: Generate messages (Anthropic compatible)
- **apply_model**: Install a model from the gallery
- **chat_completions**: Generate chat completions (OpenAI compatible)
- **create_embeddings**: Create text embeddings
- **detect_objects**: Detect objects in an image
- **face_analyze**: Analyze face demographics
- **face_identify**: Identify faces (1:N)
- **face_register**: Enroll a face into the store
- **face_verify**: Verify faces (1:1)
- **generate_image**: Supports negative prompts using | separator.

Generate images from text prompts
- **get_auth_status**: Check authentication state and providers
- **get_auth_usage**: View personal token usage
- **get_system_info**: View system and backend info
- **get_version**: Get LocalAI version
- **list_models**: List available models
- **open_responses**: Generate open responses
- **rerank_documents**: Rerank documents based on a query
- **text_to_speech**: Convert text to audio (TTS)
- **transcribe_audio**: Pass the file data or path as required by your LocalAI setup.

Transcribe audio to text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LocalAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all models available on my LocalAI instance."

**🤖 AI Agent:**
> I've retrieved the list of models. You have 'llama-3-8b', 'stablediffusion', and 'whisper-1' currently active and ready for use.

---

**👤 You:**
> "Generate a chat response using the 'llama-3' model about the benefits of local AI."

**🤖 AI Agent:**
> Using the 'llama-3' model: Local AI offers significant benefits including enhanced data privacy, reduced latency, and the ability to operate without an internet connection...

---

**👤 You:**
> "Create an image of a futuristic library using the 'stablediffusion' model."

**🤖 AI Agent:**
> I've initiated the image generation for a 'futuristic library'. The process is complete, and you can view the generated image at the provided local URL.


## Installation & Usage

To install and use the **LocalAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/localai](https://vinkius.com/mcp/localai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

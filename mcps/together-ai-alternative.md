# Together AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/together-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access 100+ open-source models for chat, image generation, and fine-tuning. Power your AI agents with Llama 3.3, Flux, and more.

## Description
Connect **Together AI** to your AI agent to leverage the world's fastest inference cloud for open-source models. This server provides a comprehensive suite of tools for generative AI, from text and image creation to advanced fine-tuning and batch processing.

### What you can do

- **Inference & Chat** — Generate high-quality responses using models like Llama 3.3, Qwen, and Mixtral via chat or text completions.
- **Media Generation** — Create stunning images and videos from text prompts using state-of-the-art models like Flux and Stable Diffusion.
- **Audio Services** — Convert text to speech (TTS) or transcribe audio files (STT) with speaker identification.
- **Advanced RAG** — Generate vector embeddings and rerank documents to build high-performance search and retrieval systems.
- **Model Management** — Manage fine-tuning jobs, dedicated endpoints, and file uploads for custom model training.
- **Batch Processing** — Handle large-scale asynchronous workloads efficiently using the Batch API.

### How it works

1. Subscribe to this server
2. Enter your Together AI API Key
3. Start building with the most powerful open-source models directly from your MCP-compatible client

### Who is this for?

- **AI Developers** — integrate cutting-edge LLMs and image models into your applications without managing infrastructure
- **Data Scientists** — fine-tune models on custom datasets and manage checkpoints seamlessly
- **Product Teams** — prototype and scale AI features using a unified, high-performance API


## Available Tools
- **create_audio_speech**: Text-to-Speech (TTS) generation
- **create_audio_transcription**: Transcriptions (STT) from audio file
- **cancel_batch**: Cancel a running batch job
- **create_chat_completion**: 3-70B-Instruct-Turbo.

Generate a model response for a given chat conversation
- **create_batch**: Create a new asynchronous batch job
- **create_endpoint**: Create a dedicated endpoint for predictable performance
- **create_fine_tune**: Create a fine-tuning job
- **delete_endpoint**: Delete a dedicated endpoint
- **delete_file**: Delete an uploaded file
- **delete_fine_tune**: Delete a fine-tuning job
- **create_embeddings**: Turn text into vector embeddings
- **get_batch**: Get details of a specific batch job
- **get_endpoint**: Get details of a specific dedicated endpoint
- **get_file**: Retrieve metadata for a specific file
- **get_fine_tune**: Get details of a specific fine-tuning job
- **create_image_generation**: Generate images from text prompts
- **list_batches**: List all batch jobs
- **list_endpoints**: List all dedicated endpoints
- **list_files**: List all uploaded files
- **list_fine_tune_checkpoints**: List checkpoints for a fine-tuning job
- **list_fine_tunes**: List all fine-tuning jobs
- **list_models**: List all available models on Together AI
- **create_rerank**: Reorder documents by relevance to a query
- **create_text_completion**: Generate text completions for a given prompt
- **update_endpoint**: Update a dedicated endpoint (Start/Stop/Scale)
- **upload_file**: Upload a file for fine-tuning, evals, or batch inference
- **create_video_generation**: Create videos from text or image prompts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Together AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a chat completion using meta-llama/Llama-3.3-70B-Instruct-Turbo explaining quantum computing."

**🤖 AI Agent:**
> I've initiated the request to Llama-3.3-70B. Quantum computing uses qubits to perform calculations that are impossible for classical computers by leveraging superposition and entanglement...

---

**👤 You:**
> "Create an image of a futuristic laboratory using the black-forest-labs/FLUX.1-schnell model."

**🤖 AI Agent:**
> Generating image... I've successfully created the image of a futuristic laboratory. You can access the result at the provided URL or as a base64 string.

---

**👤 You:**
> "List all available models on Together AI."

**🤖 AI Agent:**
> Fetching model list... You have access to over 100 models, including Llama-3.3-70B, Mixtral-8x7B, Flux.1, and various embedding models. Would you like to filter by type?


## ❓ FAQ

**Q: How do I generate a chat response using a specific model like Llama 3.3?**
Use the `create_chat_completion` tool. Specify the model name (e.g., 'meta-llama/Llama-3.3-70B-Instruct-Turbo') and provide an array of messages. The agent will return the generated response from the model.

**Q: Can I create images from text prompts with this server?**
Yes! Use the `create_image_generation` tool. You can specify the model, the prompt description, and optional parameters like width, height, and steps to get high-quality visual outputs.

**Q: How can I check the status of my asynchronous batch jobs?**
You can use `list_batches` to see all your current batch jobs or `get_batch` with a specific Job ID to retrieve detailed status and results for a particular task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/together-ai-alternative](https://vinkius.com/mcp/together-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Together AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `together-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Together AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "together-ai-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

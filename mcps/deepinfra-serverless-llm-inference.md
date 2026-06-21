# DeepInfra (Serverless LLM Inference) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepinfra-serverless-llm-inference)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Run top-tier LLMs, image generation, and embeddings via DeepInfra's serverless infrastructure directly from your AI agent.

## Description
Connect to **DeepInfra** to access a massive library of open-source models including DeepSeek, Llama 3, and FLUX. This MCP server provides high-performance, serverless inference for text, images, and specialized tasks.

### What you can do

- **Chat Completions** — Generate text using state-of-the-art models like DeepSeek-V3 or Llama-3.3-70B with full control over temperature and tokens.
- **Image Generation** — Create stunning visuals using models like FLUX-1 or Stable Diffusion by simply providing a text prompt.
- **Text Embeddings** — Convert text into high-dimensional vectors for RAG (Retrieval-Augmented Generation) or semantic search.
- **Native Inference** — Access specialized models for speech-to-text (Whisper), OCR, or custom deployments that don't follow standard OpenAI specs.

### How it works

1. Subscribe to this server
2. Enter your DeepInfra API Token
3. Start querying world-class AI models from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate powerful LLMs into your coding workflow without managing GPU infrastructure.
- **Content Creators** — generate high-quality images and text variations directly within your workspace.
- **Data Engineers** — build semantic search pipelines using serverless embedding endpoints.


## Available Tools
- **create_embedding**: Create embeddings for text via DeepInfra
- **generate_image**: Generate an image from a text prompt via DeepInfra
- **create_chat_completion**: Provide model name (e.g., deepseek-ai/DeepSeek-V3) and messages array.

Create a chat completion using an LLM via DeepInfra
- **run_native_inference**: Useful for models not covered by OpenAI spec (e.g., speech-to-text, OCR, video generation, or private deployments).

Run native inference for a specific model on DeepInfra


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeepInfra (Serverless LLM Inference)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a chat completion using deepseek-ai/DeepSeek-V3 to explain quantum entanglement."

**🤖 AI Agent:**
> I'll use the `create_chat_completion` tool with the DeepSeek-V3 model to generate a detailed explanation of quantum entanglement for you.

---

**👤 You:**
> "Create an image of a cyberpunk city at night using black-forest-labs/FLUX-1-schnell."

**🤖 AI Agent:**
> I'm calling the `generate_image` tool with the FLUX-1-schnell model and your cyberpunk prompt. One moment while the image is generated.

---

**👤 You:**
> "Generate embeddings for the text 'Artificial Intelligence is transforming the world' using BAAI/bge-large-en-v1.5."

**🤖 AI Agent:**
> I'll process that text through the `create_embedding` tool using the BGE model to get the vector representation.


## ❓ FAQ

**Q: Which LLM models can I use with the chat tool?**
You can use any model hosted on DeepInfra, such as `deepseek-ai/DeepSeek-V3` or `meta-llama/Llama-3.3-70B-Instruct`, by passing the model name to the `create_chat_completion` tool.

**Q: How do I generate images using FLUX or Stable Diffusion?**
Use the `generate_image` tool. Simply provide the model name (e.g., `black-forest-labs/FLUX-1-schnell`) and your text prompt to receive the generated image URL.

**Q: What is the 'run_native_inference' tool used for?**
It is used for models that don't follow the OpenAI chat/image spec, such as audio transcription (Whisper), specialized OCR models, or your own private model deployments on DeepInfra.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepinfra-serverless-llm-inference](https://vinkius.com/mcp/deepinfra-serverless-llm-inference)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeepInfra (Serverless LLM Inference)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deepinfra-serverless-llm-inference` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeepInfra (Serverless LLM Inference)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepinfra-serverless-llm-inference": {
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

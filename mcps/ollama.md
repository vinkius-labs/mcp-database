# Ollama MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ollama)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Run LLM models via Ollama cloud API — generate completions, chat with multimodal models, create embeddings, and inspect model details from any AI agent.

## Description
Connect your **Ollama** API key to any AI agent and run large language models through natural conversation.

### What you can do

- **Text Generation** — Generate completions from any model (Gemma, GPT-OSS, Qwen, Llama) with support for images, structured outputs (JSON schema), system prompts, and thinking mode
- **Chat Conversations** — Have multi-turn conversations with models, including multimodal inputs (vision), tool calling (function calling), and thinking output
- **Embeddings** — Generate vector embeddings for semantic search, retrieval-augmented generation (RAG), and similarity matching
- **Model Discovery** — List all available models, inspect detailed architecture info (parameters, capabilities, quantization, tokenizer settings)
- **Running Model Status** — See which models are currently loaded in memory, their VRAM usage, and when they'll be unloaded
- **OpenAI Compatibility** — Use OpenAI-compatible endpoints (/v1/chat/completions, /v1/completions, /v1/embeddings, /v1/responses) for drop-in compatibility with existing OpenAI SDK consumers
- **Version Diagnostics** — Check the Ollama server version for compatibility and troubleshooting

### How it works

1. Subscribe to this server
2. Enter your Ollama API key (create one at https://ollama.com/settings/keys)
3. Start running models from Claude, Cursor, or any MCP-compatible client

Your AI acts as a gateway to Ollama's model library — generate text, have conversations, create embeddings, and explore models without writing a single line of code.

### Who is this for?

- **Developers** — prototype with different LLM models via natural language instead of reading API docs
- **AI Engineers** — test model capabilities, generate embeddings, and compare outputs across models
- **Data Teams** — create embeddings for RAG pipelines and semantic search applications
- **Product Teams** — explore which models support vision, tools, and thinking capabilities before integrating


## Available Tools (12)
- **chat**: Supports multimodal inputs (images as base64), tool calling, structured outputs (JSON schema), thinking mode, and model options. Pass the full messages array as JSON. Uses stream=false for a single complete response.

Generate a chat message in a conversation
- **generate_embeddings**: Supports single text or array of texts, optional truncation for long inputs, and configurable output dimensions. Use for semantic search, retrieval, and RAG applications.

Generate vector embeddings from text using a model
- **generate**: Supports images (base64), structured outputs (JSON schema), system prompts, thinking mode, and model options (temperature, top_p, seed, etc.). Uses stream=false for a single complete response.

Generate a text completion from a model
- **get_version**: Useful for diagnostics and compatibility checks.

Get the Ollama server version
- **list_models**: List all available models
- **list_running_models**: Includes model name, size, VRAM usage, digest, context length, and expiry time (when the model will be unloaded).

List models currently loaded in memory
- **openai_chat_completions**: Supports messages, tools, temperature, max_tokens, seed, response_format, vision (image_url), and reasoning_effort. Uses stream=false for a single complete response.

Generate chat completions via the OpenAI-compatible endpoint
- **openai_completions**: Supports prompt, temperature, max_tokens, seed, stop sequences, and suffix (for fill-in-the-middle). Uses stream=false for a single complete response.

Generate text completions via the OpenAI-compatible endpoint
- **openai_embeddings**: Compatible with the OpenAI embeddings API. Supports input as string or array of strings, optional encoding_format and dimensions.

Generate embeddings via the OpenAI-compatible endpoint
- **openai_list_models**: Returns model IDs, creation timestamps, and ownership info. Useful when using OpenAI SDKs that require this endpoint.

List models via the OpenAI-compatible endpoint
- **openai_responses**: Compatible with the OpenAI Responses API. Uses stream=false for a single complete response.

Generate responses via the OpenAI Responses API endpoint
- **show_model_details**: Get detailed information about a specific model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ollama** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a response from gemma4 for the prompt 'Why is the sky blue?'"

**🤖 AI Agent:**
> Generating with gemma4... The sky appears blue because of a phenomenon called Rayleigh scattering. As sunlight enters Earth's atmosphere, the shorter blue wavelengths of light are scattered more than other colors by the molecules in the air. This scattered blue light comes to our eyes from all directions, making the sky appear blue.

---

**👤 You:**
> "List all available models and show me which ones support vision."

**🤖 AI Agent:**
> Found 12 models. Vision-capable models: gemma4 (8B, Q4_K_M, supports completion + vision), qwen3-vl:8b (8B, supports completion + vision + tools), and gpt-oss:20b (20B, supports completion + tools + thinking). The remaining 9 models support text completion only. Would you like detailed architecture info for any specific model?

---

**👤 You:**
> "Create embeddings for the text 'The quick brown fox jumps over the lazy dog' using nomic-embed-text."

**🤖 AI Agent:**
> Generated 768-dimensional embeddings for the input text using nomic-embed-text. The embedding vector has been created successfully. Processing took 8 tokens in the prompt evaluation. Would you like me to generate embeddings for multiple texts at once, or adjust the output dimensions?


## ❓ FAQ

**Q: How do I get my Ollama API key?**
Visit the [Ollama API keys page](https://ollama.com/settings/keys) to create or manage your API key. Once created, copy it and paste it into the API key field in the setup wizard. The key is used as a Bearer token in the Authorization header for all requests to https://ollama.com/api. API keys don't currently expire, but you can revoke them at any time.

**Q: Which models are available through this MCP?**
All models available on ollama.com are accessible, including Gemma, GPT-OSS, Qwen, Llama, and many others. Use `list_models` to see all available models, and `show_model_details` to inspect a model's capabilities (completion, vision, tools), parameter size, quantization level, and architecture details.

**Q: Can my AI use vision models to analyze images?**
Yes! The `generate` and `chat` tools support image inputs as base64-encoded strings. Use a vision-capable model (check with `show_model_details` — look for 'vision' in capabilities) and pass images in the request. The OpenAI-compatible `openai_chat_completions` tool also supports image_url content parts for vision models.

**Q: What is the difference between native and OpenAI-compatible endpoints?**
The native Ollama endpoints (`generate`, `chat`, `embed`) offer the full feature set including thinking mode, keep_alive control, and detailed response metadata (token counts, durations). The OpenAI-compatible endpoints (`/v1/chat/completions`, `/v1/completions`, `/v1/embeddings`, `/v1/responses`) provide drop-in compatibility for existing applications built with the OpenAI SDK — they use the same request/response format as OpenAI's API.

**Q: Does this MCP support tool calling (function calling)?**
Yes. The `chat` tool supports tool calling — pass a JSON array of tool definitions in the `tools_json` parameter. The model will return tool calls in the response when it determines a function should be invoked. The OpenAI-compatible `openai_chat_completions` tool also supports tools via the `tools_json` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ollama](https://vinkius.com/mcp/ollama)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ollama** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ollama` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ollama** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ollama": {
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

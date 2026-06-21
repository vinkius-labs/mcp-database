# SambaNova (AI Inference) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sambanova-ai-inference)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

High-speed AI inference for Llama 3, DeepSeek, and MiniMax models via SambaNova's ultra-fast SN40L chips.

## Description
Connect to **SambaNova Cloud** to run the world's fastest open-source models directly from your AI agent. Leverage the power of SambaNova's DataScale and SN40L infrastructure to achieve record-breaking tokens-per-second.

### What you can do

- **Chat Completions** — Generate high-quality responses using state-of-the-art models like Meta-Llama-3.3-70B-Instruct and DeepSeek-V3.1.
- **Agentic Responses** — Use the specialized `create_response` tool for stateless, typed outputs designed specifically for agentic workflows.
- **Vector Embeddings** — Generate high-dimensional text representations for RAG (Retrieval-Augmented Generation) using E5-Mistral-7B-Instruct.
- **Advanced Sampling** — Fine-tune outputs with temperature, top_p, top_k, and seed parameters for deterministic and creative results.

### How it works

1. Subscribe to this server
2. Enter your SambaNova Cloud API Key
3. Start querying high-performance models from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — building real-time applications that require low-latency inference and high throughput.
- **Developers** — looking for a cost-effective and faster alternative to standard LLM providers.
- **Data Scientists** — generating embeddings for large-scale knowledge bases at scale.


## Available Tools
- **create_chat_completion**: Compatible with OpenAI Chat Completions API.

Create a chat completion using SambaNova models
- **create_embedding**: Available on SambaStack.

Create embeddings using SambaNova
- **create_response**: Returns typed output items.

Create a response using SambaNova Responses API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SambaNova (AI Inference)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Use create_chat_completion with Meta-Llama-3.3-70B-Instruct to explain how SN40L chips work."

**🤖 AI Agent:**
> I'll generate that explanation for you using Llama 3.3 on SambaNova. [The model explains the Reconfigurable Dataflow Architecture of SN40L...]

---

**👤 You:**
> "Generate an embedding for the sentence 'SambaNova is the fastest inference platform' using E5-Mistral-7B-Instruct."

**🤖 AI Agent:**
> I've generated the embedding vector for your text. It contains 4096 dimensions (example) ready for your vector database.

---

**👤 You:**
> "Use create_response with MiniMax-M2.7 to process this conversation history."

**🤖 AI Agent:**
> Processing the agentic workflow with MiniMax... I've returned the structured response items based on the input history provided.


## ❓ FAQ

**Q: Which models are available for chat completions?**
You can use `create_chat_completion` with models like Meta-Llama-3.3-70B-Instruct, DeepSeek-V3.1, and MiniMax-M2.5 for high-speed text generation.

**Q: Can I generate embeddings for my RAG pipeline?**
Yes! Use the `create_embedding` tool with models like E5-Mistral-7B-Instruct to create vectorized representations of your text data.

**Q: What is the difference between create_chat_completion and create_response?**
`create_chat_completion` follows the standard OpenAI chat format, while `create_response` is a stateless API designed specifically for agentic workflows, returning typed output items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sambanova-ai-inference](https://vinkius.com/mcp/sambanova-ai-inference)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SambaNova (AI Inference)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sambanova-ai-inference` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SambaNova (AI Inference)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sambanova-ai-inference": {
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

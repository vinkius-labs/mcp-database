# Eden AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eden-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access 100+ AI models through a single API — route LLMs, generate embeddings, and execute specialized AI tasks like OCR and translation.

## Description
Connect **Eden AI** to your AI agent and unlock the power of over 100 leading AI providers through a single, unified interface. Orchestrate models from OpenAI, Google, Anthropic, and more without managing multiple API keys.

### What you can do

- **LLM Routing** — Use `chat_completions` with smart routing (@edenai) or specify specific provider/model combinations for conversational tasks.
- **Specialized AI Experts** — Execute synchronous or asynchronous tasks like OCR, Translation, Image Generation, and Speech-to-Text using `universal_ai_sync` and `universal_ai_async`.
- **Embeddings & Search** — Convert text into numerical vectors with `create_embedding` and explore available models via `list_embedding_models`.
- **File Management** — Upload, list, and delete files in Eden AI's persistent storage to provide context for specialized AI features.
- **Usage Monitoring** — Keep track of your consumption and available balance with `check_credits`.

### How it works

1. Subscribe to this server
2. Enter your Eden AI API Key
3. Start querying dozens of AI providers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — quickly test and compare different models (GPT-4, Claude 3, Gemini) without rewriting integration code
- **Automation Engineers** — build complex workflows involving OCR, translation, and audio processing using a single API standard
- **Data Scientists** — generate embeddings across various providers to find the best fit for RAG or semantic search applications


## Available Tools (13)
- **chat_completions**: Use @edenai for smart routing or specify provider/model.

Create a chat completion using Eden AI LLM routing
- **create_embedding**: Convert text into numerical vectors
- **create_stateful_response**: Create a stateful chat response that stores history server-side
- **delete_files**: Delete files from Eden AI storage
- **get_async_job**: Get the status and results of an asynchronous Universal AI job
- **monitor_consumption**: Monitor API consumption and costs
- **universal_ai_async**: Start an asynchronous expert model job (e.g., Speech-to-Text)
- **universal_ai_sync**: Model format: feature/subfeature/provider[/model]

Execute synchronous expert models (OCR, Translation, Image Gen)
- **upload_file**: Upload a file to Eden AI persistent storage
- **check_credits**: Check current Eden AI credit balance
- **list_files**: List all files uploaded to Eden AI
- **create_custom_token**: Create a custom API token with specific constraints
- **list_embedding_models**: List available embedding models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eden AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a chat completion using openai/gpt-4o via Eden AI."

**🤖 AI Agent:**
> I've initiated the chat completion with GPT-4o. The model responded: 'Hello! How can I assist you today with Eden AI's unified interface?'

---

**👤 You:**
> "Generate an image of a futuristic city using image/generation/openai/dall-e-3."

**🤖 AI Agent:**
> Executing the image generation task... I've successfully generated the image of a futuristic city via DALL-E 3. You can access the result at the provided URL.

---

**👤 You:**
> "Check my current Eden AI credit balance."

**🤖 AI Agent:**
> I've checked your account. You currently have 45.50 credits remaining in your Eden AI balance.


## ❓ FAQ

**Q: How can I use Eden AI's smart routing to find the best model for a chat?**
Simply use the `chat_completions` tool and set the `model` parameter to `@edenai`. This will automatically route your request to the most suitable provider based on performance and cost.

**Q: How do I handle long-running AI tasks like Speech-to-Text?**
Use the `universal_ai_async` tool to start the job. You will receive a job ID which you can then use with the `get_async_job` tool to check the status and retrieve the final results once finished.

**Q: Can I manage the files I upload for AI processing?**
Yes. You can use `upload_file` to send data, `list_files` to see everything in your storage, and `delete_files` to remove them when they are no longer needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eden-ai-alternative](https://vinkius.com/mcp/eden-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eden AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eden-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eden AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eden-ai-alternative": {
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

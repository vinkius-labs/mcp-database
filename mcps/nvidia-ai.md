# NVIDIA AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nvidia-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access LLMs, embeddings, code generation, and reasoning via NVIDIA API Catalog.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NVIDIA AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate Python code for a REST API with FastAPI."

**🤖 AI Agent:**
> Generated code: `from fastapi import FastAPI
app = FastAPI()

@app.get('/items')
async def get_items():
    return {'items': []}`

---

**👤 You:**
> "Translate 'Hello, how are you?' to Japanese."

**🤖 AI Agent:**
> こんにちは、お元気ですか？ (Konnichiwa, ogenki desu ka?)

---

**👤 You:**
> "Summarize: The quarterly report shows revenue grew 15% YoY..."

**🤖 AI Agent:**
> Q3 revenue increased 15% year-over-year, driven by strong demand in AI and cloud services.


## ❓ FAQ

**Q: Which AI models are available?**
The NVIDIA API Catalog offers Llama 3.1 (8B, 70B, 405B), Mistral, CodeLlama, Gemma, Nemotron, and many more. Use the `list_models` tool to see all available models.

**Q: How do I get an NVIDIA API Key?**
Sign up at [**build.nvidia.com**](https://build.nvidia.com), go to your account settings, and generate an API key. The Developer Program includes free inference credits.

**Q: Can I generate code in specific languages?**
Yes! The `generate_code` tool lets you specify the programming language (Python, JavaScript, TypeScript, Java, etc.) for better results.

**Q: Are there usage limits on the free tier?**
Yes, the NVIDIA Developer Program provides free inference credits. Once exhausted, you can upgrade to a paid plan for higher throughput. Check your usage dashboard at build.nvidia.com.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nvidia-ai](https://vinkius.com/mcp/nvidia-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NVIDIA AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nvidia-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NVIDIA AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nvidia-ai": {
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

# Baidu Qianfan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-qianfan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Baidu Qianfan AI models — manage chat completions, embeddings, and prompt templates directly from any AI agent.

## Description
Connect your AI agents to **Baidu Qianfan** (百度千帆), the enterprise-grade LLM platform. This MCP provides 10 tools to automate interactions with Ernie Bot and other foundation models, including chat completions, vector embeddings, and prompt engineering.

### What you can do

- **Model Interaction** — Trigger chat completions with Ernie Bot (Turbo/Speed/4.0) using persistent context
- **Vector Embeddings** — Generate semantic embeddings for text to power RAG and search workflows
- **Prompt Engineering** — Manage and retrieve centralized prompt templates for consistent model outputs
- **Image Generation** — Trigger Text-to-Image tasks using Baidu's advanced diffusion models
- **Usage Monitoring** — Track token consumption and manage model service status programmatically

### How it works

1. Subscribe to this server
2. Log in to the [**Baidu Qianfan Console**](https://console.bce.baidu.com/qianfan/)
3. Create an application to obtain your **API Key** and **Secret Key**
4. Enable the models you wish to use (e.g., Ernie-4.0-8K)
5. Insert your credentials into the fields below to start managing your Baidu AI workflows.

### Who is this for?

- **AI Developers** — automate the comparison of different Ernie model versions
- **System Integrators** — bridge enterprise applications with Baidu's high-performance Chinese LLMs
- **Knowledge Managers** — build robust RAG pipelines using Qianfan's embedding and chat services


## Available Tools
- **get_embeddings**: Generate vector embeddings for text
- **list_train_jobs**: List model training jobs
- **chat_completions**: Requires model endpoint name.

Send a message to a Baidu Qianfan model
- **list_datasets**: List uploaded datasets
- **list_models**: List available model services
- **text_to_image**: Generate an image from a text prompt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baidu Qianfan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chat with Ernie Bot 4.0 and ask 'Write a formal apology letter for a late shipment'."

**🤖 AI Agent:**
> Connecting to Qianfan engine... Ernie 4.0 responded: 'Subject: Formal Apology... We sincerely regret the delay in your shipment #12345...' Would you like me to refine the tone?

---

**👤 You:**
> "Generate embeddings for the text 'The quick brown fox jumps over the lazy dog'."

**🤖 AI Agent:**
> Retrieving embeddings... I've generated a 384-dimensional vector for your input using Baidu's embedding-v1 model. The data is ready for your RAG search index.

---

**👤 You:**
> "List all my prompt templates in Qianfan."

**🤖 AI Agent:**
> Fetching templates... I found 3 templates: 1. Code-Review-Expert (ID: tp_1), 2. Creative-Writer (ID: tp_2), 3. SQL-Generator (ID: tp_3). Which one would you like to use?


## ❓ FAQ

**Q: Which version of Ernie Bot should I use for chat?**
For high performance and reasoning, use `ernie-4.0-8k`. For faster response times and cost efficiency, `ernie-speed-128k` or `ernie-lite-8k` are excellent choices.

**Q: Can I automatically generate embeddings for RAG?**
Yes! Use the `get_embeddings` tool with your text input. The agent will retrieve the vector representations from Baidu's embedding models, ready for indexing in your vector database.

**Q: How do I use prompt templates from the console?**
Use the `list_prompt_templates` tool to find your configured templates. You can then retrieve specific details using `get_prompt_template` to maintain consistency across your AI workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-qianfan](https://vinkius.com/mcp/baidu-qianfan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baidu Qianfan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `baidu-qianfan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baidu Qianfan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baidu-qianfan": {
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

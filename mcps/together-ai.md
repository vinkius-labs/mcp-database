# Together AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/together-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate code, evaluate embeddings, and deploy open-source LLMs instantly from your local agent via Together AI's infrastructure.

## Description
Connect your **Together AI** account to any AI agent and integrate bleeding-edge open-source models seamlessly into your workflow. Harness world-class inference speeds to query Llama, Mixtral, and more, or orchestrate specialized model fine-tuning jobs straight from your chat environment.

### What you can do

- **Model Discovery** — Explore and list all currently supported models on the Together network, identifying the best engine for any NLP or vision task
- **Conversational AI** — Run chat completion cycles on advanced models simply by supplying a model ID directly from the chat prompt
- **Vector Storage Preparation** — Generate instant rich embeddings for input texts, ready to populate your analytical databases
- **Creative Media** — Instruct external diffusion models to generate images using detailed physical descriptions
- **Custom Fine-Tuning** — Provision custom training runs by indicating a base framework and dataset file, alongside tracking existing job statuses

### How it works

1. Sign up for this integration
2. Open your api.together.xyz control panel and fetch a developer API Key
3. Plug the key above, specify models to your agent, and enjoy sub-second serverless inference directly inside your command interface

### Who is this for?

- **AI Developers** — Orchestrate fine-tuning parameters and launch jobs to the compute cluster without CLI switching
- **Software Engineers** — Use the provider to test completions using alternative open-source solutions (e.g., Llama 3) natively in code editors
- **Machine Learning Engineers** — Bulk-generate vectors from raw logs using embedding models attached straight to their main conversational agent


## Available Tools
- **chat_completion**: Provide a model ID and a JSON array of messages.

Executes a chat completion using Together AI models
- **text_completion**: Provide a model ID and a prompt.

Executes a base text completion
- **create_finetune_job**: Provide a base model ID and a training file ID.

Creates a new fine-tuning job
- **generate_embeddings**: Provide a model ID and a JSON array of strings.

Generates vector embeddings for input texts
- **generate_image**: Provide a model ID and descriptive prompt.

Generates an image from a text prompt
- **list_finetune_jobs**: Lists all fine-tuning jobs
- **list_available_models**: Lists all AI models available on Together AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Together AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the models currently available on Together AI."

**🤖 AI Agent:**
> I've fetched 132 available models. Here are the top chat models:
- meta-llama/Llama-2-70b-chat-hf
- mistralai/Mixtral-8x7B-Instruct-v0.1
- google/gemma-7b-it
Ask if you want the embedding or image models only.

---

**👤 You:**
> "Generate an embedding array using model `togethercomputer/m2-bert-80M-8k-retrieval` for the sentence 'The cat sat on the mat'."

**🤖 AI Agent:**
> Embeddings generated successfully. Dimensions: 768. Sample values:
[-0.0124, 0.0411, 0.0812, ... -0.0123]


## ❓ FAQ

**Q: Where do I obtain my Together AI API Key?**
Log in to the developer portal via `api.together.xyz/settings/api-keys`. If you do not have an existing key, click **Create API Key**. This token enables the execution of remote inferences spanning their hosted clusters securely.

**Q: Do I have to pay to use Together models through the agent?**
Yes. This connector simply routes your instructions to Together AI. Any tokens consumed during chat completion, embeddings, images generation, or fine-tuning workloads are billed directly to your registered Together AI account balance according to their official compute pricing models.

**Q: Can I access free models on Together AI?**
Yes! Together AI frequently offers free tiers for certain open-source models intended for experimentation and research. You can query these directly from your agent without depleting your account balance, though specific free-tier rate limits will apply.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/together-ai](https://vinkius.com/mcp/together-ai)
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
3. Set Type to "SSE", enter `together-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Together AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "together-ai": {
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

# Predibase (LLM Serving & Finetuning) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/predibase-llm-serving-finetuning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deploy and query fine-tuned LLMs via Predibase — run inference, classify text, and monitor deployment metrics directly from your AI agent.

## Description
Connect your **Predibase** account to any AI agent to manage high-performance LLM serving and fine-tuning workflows. Predibase provides a unified interface for serverless LLM deployment and LoRA adapter management.

### What you can do

- **LLM Inference** — Generate text or chat completions using `generate_text`, `chat_completion`, and `completion` tools.
- **Fine-tuning Integration** — Dynamically apply LoRA adapters during inference using the `adapter_id` parameter in generation tasks.
- **Text Classification** — Perform batch classification tasks with the `classify` tool for structured data workflows.
- **Deployment Monitoring** — Check the status of your endpoints with `get_health`, `get_info`, and `get_metrics`.
- **Structured Output** — Enforce JSON schemas on model responses for reliable downstream automation.

### How it works

1. Subscribe to this server
2. Provide your Predibase API Token and Tenant ID
3. Start querying your deployments from Claude, Cursor, or any MCP client

### Who is this for?

- **AI Engineers** — deploy and test fine-tuned models without leaving the chat interface
- **Data Scientists** — monitor inference metrics and health of production deployments
- **Developers** — integrate high-performance LLM capabilities into apps with structured JSON output


## Available Tools (7)
- **generate_text**: Generate text using a deployed LLM
- **get_health**: Check health status of the inference endpoint
- **get_info**: Get inference endpoint metadata
- **get_metrics**: Get Prometheus metrics for the deployment
- **chat_completion**: Create a chat completion (OpenAI compatible)
- **classify**: Batch classification for one or more inputs
- **completion**: Create a completion (OpenAI compatible)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Predibase (LLM Serving & Finetuning)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a summary of this text using the 'llama-3-70b' deployment."

**🤖 AI Agent:**
> I'll use the `generate_text` tool on your 'llama-3-70b' deployment. Processing the input prompt now...

---

**👤 You:**
> "Check the health and metrics for my 'customer-support-llm' deployment."

**🤖 AI Agent:**
> I am calling `get_health` and `get_metrics` for 'customer-support-llm'. The endpoint is currently healthy and processing 12 requests per minute.

---

**👤 You:**
> "Classify these three reviews using our sentiment model deployment."

**🤖 AI Agent:**
> Running the `classify` tool for your inputs. Results: Review 1 (Positive), Review 2 (Negative), Review 3 (Neutral).


## ❓ FAQ

**Q: Can I use my fine-tuned adapters with this server?**
Yes. When using the `generate_text` tool, you can provide an `adapter_id` to apply your specific fine-tuned LoRA adapter to the base model deployment.

**Q: How do I monitor the performance of my Predibase deployment?**
Use the `get_metrics` tool to scrape Prometheus-formatted metrics or `get_info` to retrieve metadata like model ID and device type.

**Q: Does this support structured JSON responses?**
Absolutely. The `generate_text` tool includes a `schema` parameter that allows you to pass a JSON schema to ensure the model output follows a specific structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/predibase-llm-serving-finetuning](https://vinkius.com/mcp/predibase-llm-serving-finetuning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Predibase (LLM Serving & Finetuning)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `predibase-llm-serving-finetuning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Predibase (LLM Serving & Finetuning)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "predibase-llm-serving-finetuning": {
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

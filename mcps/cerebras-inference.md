# Cerebras Inference MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cerebras-inference)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access lightning-fast AI inference via Cerebras Wafer-Scale Engine — generate chat completions, manage models, and run batch jobs at record speeds.

## Description
Connect to the **Cerebras Inference** platform to leverage the world's fastest AI inference. This MCP server allows your AI agent to interact with state-of-the-art models like Llama 3.1 and others using the Cerebras Wafer-Scale Engine (WSE) for unprecedented performance.

### What you can do

- **Chat & Text Completions** — Generate high-speed responses using `create_chat_completion` and `create_completion` with support for streaming and tool calling.
- **Model Discovery** — Explore available models and their specific details using `list_models` and `get_model` to choose the best fit for your task.
- **Batch Processing** — Handle large-scale workloads asynchronously with `create_batch`, `list_batches`, and `cancel_batch` for efficient data processing.
- **File Management** — Upload and manage JSONL files for batch jobs using `upload_file` and `list_files` directly from your agent.
- **Performance Metrics** — Monitor your usage and performance metrics to optimize your inference workflows.

### How it works

1. Subscribe to this server
2. Enter your Cerebras API Key
3. Start generating tokens at speeds you've never seen before in Claude, Cursor, or any MCP-compatible client.

### Who is this for?

- **AI Developers** — build and test applications with near-instant model responses to maintain development momentum.
- **Data Scientists** — run large-scale batch inference on massive datasets using the asynchronous batch API.
- **Product Teams** — integrate high-performance LLMs into production environments where latency is a critical factor.


## Available Tools (15)
- **cancel_batch**: Cancel a batch job
- **upload_file**: Upload a JSONL file for Batch processing
- **create_chat_completion**: Generate conversational responses using a structured message format
- **create_completion**: Generate text continuations from a single prompt string
- **create_batch**: Create a batch job for asynchronous processing
- **delete_file**: Delete a file
- **get_batch**: Retrieve status of a batch job
- **get_file_content**: Download raw content of a file
- **get_file**: Retrieve metadata for a specific file
- **get_metrics**: Retrieve Prometheus-formatted operational metrics
- **get_model**: Fetches details for a specific model
- **list_batches**: List all batch jobs
- **list_files**: List uploaded files
- **list_models**: Lists all currently available models
- **list_public_models**: Retrieve model details without an API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cerebras Inference** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available models on Cerebras."

**🤖 AI Agent:**
> I've retrieved the available models. You can use 'llama3.1-8b', 'llama3.1-70b', or 'gpt-oss-120b' for high-speed inference. Which one would you like to use for your request?

---

**👤 You:**
> "Generate a chat response using llama3.1-8b explaining quantum entanglement."

**🤖 AI Agent:**
> Using the `create_chat_completion` tool with model 'llama3.1-8b'... Quantum entanglement is a physical phenomenon that occurs when a group of particles are generated, interact, or share spatial proximity in a way such that the quantum state of each particle cannot be described independently...

---

**👤 You:**
> "Check the status of my batch job with ID 'batch_abc123'."

**🤖 AI Agent:**
> I've checked the status using `get_batch`. The job 'batch_abc123' is currently 'completed'. You can now retrieve the results using the file tools.


## ❓ FAQ

**Q: How do I check which models are available for inference?**
Use the `list_models` tool. It will return a list of all supported models, including high-performance options like Llama 3.1, which you can then use in `create_chat_completion`.

**Q: Can I process thousands of requests at once?**
Yes. Use `upload_file` to provide your JSONL data and then `create_batch` to start an asynchronous processing job. You can monitor progress with `get_batch`.

**Q: Does this server support tool calling and structured outputs?**
Yes. The `create_chat_completion` tool supports `tools`, `tool_choice`, and `response_format` parameters, allowing the model to interact with other functions or return valid JSON.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cerebras-inference](https://vinkius.com/mcp/cerebras-inference)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cerebras Inference** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cerebras-inference` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cerebras Inference** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cerebras-inference": {
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

# Forefront MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/forefront)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Forefront AI models directly from your agent — generate chat completions, manage fine-tuning jobs, and collect LLM outputs with pipelines.

## Description
Connect your **Forefront** account to any AI agent to harness powerful language models, manage custom fine-tuning, and orchestrate data pipelines directly through natural conversation.

### What you can do

- **Chat & Text Completions** — Generate high-quality model responses using chat-ml format or standard prompts via `create_chat_completion` and `create_completion`.
- **Fine-Tuning Management** — Kick off custom training jobs on base models with your own training and validation datasets using `create_fine_tune`.
- **Pipeline Orchestration** — Create and manage pipelines to collect LLM outputs, track samples, and organize metadata using `create_pipeline`, `list_pipelines`, `get_pipeline`, and `add_pipeline_data`.

### How it works

1. Subscribe to this server
2. Enter your Forefront API Key
3. Start generating text and managing pipelines from Claude, Cursor, or any MCP client


## Available Tools (10)
- **add_pipeline_data**: Add data samples to a pipeline
- **list_pipelines**: Returns a list of your pipelines
- **create_chat_completion**: Pass messages array in chat-ml format.

Creates a model response for the given chat conversation
- **create_completion**: Pass a single prompt string.

Creates a completion response for a given prompt
- **create_fine_tune**: Creates a fine-tuning job
- **create_pipeline_dataset**: Create a dataset from a pipeline selection
- **create_pipeline**: Create a new pipeline to collect LLM outputs
- **get_pipeline_count**: Get count of pipeline selection
- **get_pipeline_samples**: Get data samples for a pipeline selection
- **get_pipeline**: Returns a pipeline object by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forefront** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a chat completion with model 'forefront-llm' asking 'What is the capital of France?'"

**🤖 AI Agent:**
> I will call `create_chat_completion` with model 'forefront-llm' and the message 'What is the capital of France?'. The model responded: 'The capital of France is Paris.'

---

**👤 You:**
> "List all my active pipelines on Forefront."

**🤖 AI Agent:**
> I will query your pipelines using `list_pipelines`. I found 2 active pipelines: 'customer-feedback-pipeline' (ID: pipe_123) and 'qa-testing-pipeline' (ID: pipe_456).

---

**👤 You:**
> "Create a new pipeline named 'production-logs'."

**🤖 AI Agent:**
> I will call `create_pipeline` with the name 'production-logs'. The pipeline has been successfully created with ID 'pipe_789'.


## ❓ FAQ

**Q: How can I generate a model response using a chat conversation?**
You can use the `create_chat_completion` tool. Provide the model name and an array of messages in chat-ml format to receive the generated response.

**Q: Can I start a custom fine-tuning job directly from my agent?**
Yes! Use the `create_fine_tune` tool by specifying the name of your fine-tuned model, the baseModel, and the trainingDataset ID to begin training.

**Q: How do I collect LLM outputs using pipelines?**
First, create a pipeline using `create_pipeline`. Once created, you can use `add_pipeline_data` to log messages, user IDs, and custom metadata directly into that pipeline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forefront](https://vinkius.com/mcp/forefront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Forefront** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `forefront` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Forefront** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "forefront": {
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

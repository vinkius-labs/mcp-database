# OpenAI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage OpenAI resources via API — list models, monitor fine-tunes, manage batches and inspect Assistants from any AI agent.

## Description
Connect your **OpenAI** account to any AI agent and take full control of your AI resources through natural conversation.

### What you can do

- **Model Discovery** — List all available models (GPT-4, GPT-3.5, DALL-E, Whisper, Embeddings) with ownership and capability info
- **File Management** — Browse, manage and delete uploaded files used for fine-tuning and Assistants
- **Fine-Tuning** — Monitor fine-tuning jobs, check status (running, succeeded, failed) and cancel long-running jobs
- **Batch Processing** — Create, track and cancel batch jobs for cost-effective bulk API processing
- **Assistant Management** — List and inspect configured Assistants with their models, tools and instructions

### How it works

1. Subscribe to this server
2. Enter your OpenAI API Key
3. Start managing your AI resources from Claude, Cursor, or any MCP-compatible client

No more switching to the OpenAI dashboard to check fine-tune status or manage batch jobs. Your AI acts as a dedicated ML ops assistant.

### Who is this for?

- **ML Engineers** — monitor fine-tuning jobs, track batch processing and manage model files without leaving your IDE
- **DevOps** — audit uploaded files, review batch statuses and clean up unused resources
- **Product Teams** — discover available models, inspect Assistant configurations and review resource usage


## Available Tools (13)
- **cancel_batch**: Partially completed requests may still be processed. Provide the batch ID.

Cancel a running batch job
- **cancel_fine_tune**: The job status will change to "cancelled". Provide the fine-tune job ID. This is useful if you uploaded the wrong training file or want to stop a long-running job.

Cancel a running fine-tuning job
- **create_batch**: Requires the input file ID (containing JSONL requests) and the endpoint (e.g. "/v1/chat/completions"). Optionally set the completion window ("24h" default). Returns the batch with its ID for tracking.

Create a new batch processing job
- **delete_file**: Provide the file ID from list_files. WARNING: this action is irreversible and will break any fine-tunes or assistants using this file.

Delete an uploaded file from OpenAI
- **get_assistant**: Provide the assistant ID.

Get details for a specific OpenAI Assistant
- **get_batch**: Provide the batch ID.

Get details for a specific batch job
- **get_fine_tune**: Provide the fine-tune job ID.

Get details for a specific fine-tuning job
- **get_model**: g. "gpt-4o", "gpt-4o-mini", "text-embedding-3-small", "dall-e-3", "whisper-1"). Returns the model ID, owner organization, creation date and permission flags. Use this to verify a model exists and check its metadata before using it.

Get details for a specific OpenAI model
- **list_assistants**: Each Assistant shows its ID, name, instructions, model, tools (code interpreter, file search, function calling) and creation date. Use this to audit your Assistant configurations.

List OpenAI Assistants
- **list_batches**: Batches allow you to process many API requests at once at a lower cost. Each batch shows its ID, status (validating, in_progress, finalizing, completed, failed, expired, cancelled), input/output file IDs and request counts.

List batch processing jobs
- **list_files**: Files are used for fine-tuning, Assistants API and batch processing. Each file shows its ID, filename, purpose (fine-tune, assistants, batch), size and status. Optionally filter by purpose.

List files uploaded to OpenAI
- **list_fine_tunes**: Each job shows its ID, status (validating_files, queued, running, succeeded, failed, cancelled), base model, training file, created date and estimated finish time. Use this to monitor your fine-tuning pipeline.

List fine-tuning jobs
- **list_models**: 5, DALL-E, Whisper, Embedding and fine-tuned models. Each model returns its ID, owned_by (organization), creation date and permissions. Use this to discover which models are available for your account and their capabilities.

List all available OpenAI models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available GPT models."

**🤖 AI Agent:**
> I found 12 GPT models in your account: gpt-4o (owned by openai, created 2024-05), gpt-4o-mini (lightweight, cost-effective), gpt-4-turbo, gpt-4, gpt-3.5-turbo, plus several fine-tuned variants. Would you like details on any specific model?

---

**👤 You:**
> "Check the status of my latest fine-tuning job."

**🤖 AI Agent:**
> Your latest fine-tune job ftjob-abc123 is currently 'running' at 67% completion. It's training on 1,240 examples using gpt-3.5-turbo as the base model. Estimated finish is in approximately 2 hours. The training file is file-xyz789.

---

**👤 You:**
> "List all my uploaded files and their purposes."

**🤖 AI Agent:**
> You have 8 files uploaded: 3 for fine-tuning (training JSONL files), 2 for Assistants (knowledge base PDFs), 2 for batch processing (request JSONL files) and 1 vector store file. Total storage used: 45MB.


## ❓ FAQ

**Q: How do I get my OpenAI API Key?**
Log in to the [**OpenAI Platform**](https://platform.openai.com/api-keys), go to **API Keys** in the left sidebar, click **Create new secret key**, give it a name and copy the key immediately — it starts with `sk-proj-` and won't be shown again.

**Q: Can I monitor my fine-tuning jobs?**
Yes! Use `list_fine_tunes` to see all fine-tuning jobs with their status (validating_files, queued, running, succeeded, failed, cancelled). Use `get_fine_tune` with a specific job ID for detailed info including training progress, estimated finish time and result model ID. You can also cancel running jobs with `cancel_fine_tune`.

**Q: Can I manage batch processing jobs?**
Yes! Use `list_batches` to see all batch jobs, `create_batch` to submit new batches with an input file ID and endpoint, `get_batch` to check progress and `cancel_batch` to stop running jobs. Batches process requests asynchronously at a lower cost than individual API calls.

**Q: Can I list and inspect my Assistants?**
Yes! Use `list_assistants` to see all configured Assistants with their models, tools (code interpreter, file search, function calling) and instructions. Use `get_assistant` with a specific assistant ID for full details including file IDs and metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openai-alternative](https://vinkius.com/mcp/openai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenAI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenAI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openai-alternative": {
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

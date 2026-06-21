# OpenAI MCP Server

Manage OpenAI resources via API — list models, monitor fine-tunes, manage batches and inspect Assistants from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openai-alternative)

## Overview
**Category:** ai-frontier
**Tools Count:** 13

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


## Available Tools
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


## Installation & Usage

To install and use the **OpenAI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openai-alternative](https://vinkius.com/mcp/openai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

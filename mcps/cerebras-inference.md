# Cerebras Inference MCP Server

Access lightning-fast AI inference via Cerebras Wafer-Scale Engine — generate chat completions, manage models, and run batch jobs at record speeds.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cerebras-inference)

## Overview
**Category:** ai-frontier
**Tools Count:** 15

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


## Available Tools
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


## Installation & Usage

To install and use the **Cerebras Inference** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cerebras-inference](https://vinkius.com/mcp/cerebras-inference)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

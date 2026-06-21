# Forefront MCP Server

Access Forefront AI models directly from your agent — generate chat completions, manage fine-tuning jobs, and collect LLM outputs with pipelines.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/forefront)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Forefront** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forefront](https://vinkius.com/mcp/forefront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

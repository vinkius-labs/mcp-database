# Humanloop (LLM Prompt Management API) MCP Server

Manage, version, and deploy LLM prompts directly from your AI agent using the Humanloop API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/humanloop-llm-prompt-management-api)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **Humanloop** account to any AI agent to streamline your LLM operations (LLMOps). Manage your prompt library, track versions, and deploy configurations to different environments through natural conversation.

### What you can do

- **Prompt Management** — List all prompts in your organization and fetch detailed configurations for specific IDs.
- **Version Control** — Retrieve version history, update version metadata, or delete obsolete versions to keep your library clean.
- **Deployment** — Set specific prompt versions as active in environments like staging or production with a single command.
- **Logging & Execution** — Record model generations (logs) for evaluation and execute prompts with streaming support.
- **Monitoring** — Update monitoring settings and list available environments to ensure your LLM pipeline is healthy.

### How it works

1. Subscribe to this server
2. Enter your Humanloop API Key
3. Start managing your prompt engineering workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — deploy and test prompt iterations directly from the code editor without switching to the Humanloop dashboard.
- **Product Managers** — audit prompt versions and monitor model outputs to ensure quality and alignment.
- **DevOps Teams** — automate the deployment of prompt configurations across different environments.


## Available Tools
- **call_prompt_stream**: Execute a prompt and stream the response
- **delete_prompt_version**: Remove a specific version of a prompt
- **deploy_prompt**: g., production, staging).

Set a specific version as the active deployment for an environment
- **get_prompt**: Retrieve details for a specific prompt by ID
- **list_prompt_environments**: List all environments and their currently deployed versions for a prompt
- **list_prompt_versions**: Get all versions associated with a specific prompt
- **list_prompts**: Retrieve a list of all prompts in your organization
- **log_to_prompt**: Record a model generation (log) associated with a specific prompt
- **remove_deployment**: Remove a prompt version from an environment
- **update_monitoring**: Activate or deactivate Evaluators for monitoring logs within a prompt
- **update_prompt_version**: Update the name or description of a specific prompt version
- **upsert_prompt**: Create or update a prompt configuration


## Installation & Usage

To install and use the **Humanloop (LLM Prompt Management API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/humanloop-llm-prompt-management-api](https://vinkius.com/mcp/humanloop-llm-prompt-management-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

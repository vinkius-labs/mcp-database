# Dify.AI SDK MCP Server

Trigger and orchestrate Dify AI workflows, agents, and chatbots programmatically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/difyai-sdk)

## Overview
**Category:** developer-apis
**Tools Count:** 14

## Description
Connect your Vinkius agents directly to **Dify.AI**, the leading open-source LLM app development platform. With 10 exposed tools, you can execute complex Dify workflows, send messages to specialized chatbots, retrieve session histories, and submit model feedback for RLHF.

### What you can do

- **Agent Chat** — Send messages to published Dify chatbots and track conversations
- **Workflows** — Trigger background Dify workflows with dynamic JSON parameters
- **Session Management** — Rename, fetch, or delete conversation histories
- **Audit & Feedback** — Programmatically submit 'like/dislike' ratings to improve model tuning

### How it works

1. Publish your App (Chatbot or Workflow) on Dify
2. Navigate to your app's **API Access** section and generate an API API Key
3. Set the Base URL to `https://api.dify.ai/v1` (for cloud) or your own instance.

### Who is this for?

- **LLM Developers** — Integrate multi-agent orchestration by letting Vinkius agents call Dify-specialized workflows
- **Product Teams** — Monitor interactions and automate RLHF pipelines via feedback endpoints


## Available Tools
- **delete_conversation**: Delete a Dify conversation
- **submit_feedback**: Submit feedback (like/dislike) for a message
- **get_suggested_questions**: Use after receiving a chat response.

Get next suggested questions for a message
- **chat_message**: Send a chat message to a Dify Application
- **get_app_meta**: Get application meta data configuration
- **get_conversation_messages**: Get historical messages of a specific Dify conversation
- **get_conversations**: List recent conversations for a user
- **get_workflow_info**: Get basic App information
- **get_workflow_parameters**: Get required application parameters
- **rename_conversation**: Rename a Dify conversation
- **run_workflow**: Execute a Dify Workflow application
- **send_completion**: Returns the full generated text.

Send a text completion request to a Dify completion app
- **stop_chat_generation**: Only supported for streaming mode responses.

Stop an in-progress chat message generation
- **upload_file**: Upload a file via URL for multimodal understanding


## Installation & Usage

To install and use the **Dify.AI SDK** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/difyai-sdk](https://vinkius.com/mcp/difyai-sdk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Dify.AI SDK MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/difyai-sdk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-apis](../categories/developer-apis.md)

Trigger and orchestrate Dify AI workflows, agents, and chatbots programmatically.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dify.AI SDK** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my recent Dify conversations and tell me the name of the last one."

**🤖 AI Agent:**
> Your last conversation in Dify is titled 'Data Processing Bot' (ID: conv-123).


## ❓ FAQ

**Q: Does this work with self-hosted Dify?**
Yes, simply replace the Base URL credential with your own domain (e.g. `https://dify.mycompany.com/v1`).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/difyai-sdk](https://vinkius.com/mcp/difyai-sdk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dify.AI SDK** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `difyai-sdk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dify.AI SDK** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "difyai-sdk": {
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

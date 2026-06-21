# Anthropic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anthropic-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Access Claude models via Anthropic API — send messages, count tokens, manage batches and discover models from any AI agent.

## Description
Connect your **Anthropic** account to any AI agent and leverage Claude's capabilities through natural conversation.

### What you can do

- **Model Discovery** — List all available Claude models with their IDs and capabilities
- **Message API** — Send conversations to Claude models and receive responses with configurable max tokens, system prompts and temperature
- **Token Counting** — Count tokens in messages before sending to estimate costs and context window usage
- **Batch Processing** — Submit batches of independent message requests for asynchronous, cost-effective processing

### How it works

1. Subscribe to this server
2. Enter your Anthropic API Key
3. Start using Claude from Claude, Cursor, or any MCP-compatible client

No more switching between API tools to interact with Claude. Your AI acts as an LLM orchestration layer.

### Who is this for?

- **Developers** — quickly send messages to Claude, count tokens and manage batch requests without writing HTTP code
- **ML Engineers** — discover available models, compare capabilities and batch-process many prompts efficiently
- **Product Teams** — review model outputs, track token usage and manage batch processing jobs via conversation


## Available Tools
- **cancel_batch_message**: Requests that have already been completed cannot be cancelled. Provide the batch ID. This is useful if you submitted a large batch by mistake and want to stop further processing to save costs.

Cancel an in-progress batch message request
- **count_tokens**: Requires the model ID and messages array. Returns the total input token count. Useful for estimating API costs and ensuring messages fit within context limits.

Count tokens in a message before sending to Claude
- **create_batch_message**: Each request in the batch has its own model, messages, max_tokens, etc. This is more cost-effective than individual requests when you have many independent prompts to process. Returns a batch ID for tracking. Use get_batch_message to check progress.

Create a batch of message requests to Claude
- **get_batch_message**: Returns the batch status (in_progress, succeeded, expired, canceling, canceled, failed), request counts (total, succeeded, errored) and individual results. Use the batch ID returned from create_batch_message.

Get the status of a batch message request
- **list_models**: Each model returns its ID (e.g. "claude-sonnet-4-20250514"), display name, creation date and capabilities. Use this to discover which models are available and their IDs for use with the send_message tool.

List all available Anthropic Claude models
- **send_message**: Requires the model ID (e.g. "claude-sonnet-4-20250514") and messages array in JSON format. Each message must have a "role" ("user" or "assistant") and "content" (text or array of content blocks). Optionally set max_tokens (default 1024), system prompt and temperature (0-1). Returns the assistant's response text.

Send a message to Claude (Messages API)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anthropic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to Claude asking 'What is the capital of Brazil?'"

**🤖 AI Agent:**
> Claude responded: 'The capital of Brazil is Brasília. It was purpose-built to replace Rio de Janeiro as the capital in 1960, and is located in the country's central-west region.' The response used 45 tokens.

---

**👤 You:**
> "List all available Claude models."

**🤖 AI Agent:**
> Available models: claude-sonnet-4-20250514 (latest Sonnet, 200K context), claude-opus-4-20250514 (most capable, 200K context), claude-haiku-20241022 (fastest, cost-effective, 200K context). Each model has different pricing and capabilities.

---

**👤 You:**
> "Count tokens for a message asking Claude to summarize a 500-word article."

**🤖 AI Agent:**
> The message would use approximately 547 input tokens (45 for the prompt + 502 for the article text). With a typical response of 150 tokens, the total would be ~697 tokens for this conversation turn.


## ❓ FAQ

**Q: How do I get an Anthropic API Key?**
Log in to the [**Anthropic Console**](https://console.anthropic.com), go to **Account Settings > API Keys** and click **Create Key**. Copy the key immediately — it starts with `sk-ant-` and won't be shown again. You can also create workspace-scoped keys to control spending by use case.

**Q: What models are available?**
Use the `list_models` tool to see all available Claude models. Current models include Claude Sonnet 4, Claude Opus 4 and Claude Haiku variants, each with different capabilities, context windows and pricing. The model ID format is like `claude-sonnet-4-20250514`.

**Q: Can I send multi-turn conversations?**
Yes! Pass a messages array with alternating 'user' and 'assistant' roles. Each message has a 'role' and 'content' field. Claude will continue the conversation based on the full message history. Example: [{"role":"user","content":"Hello"},{"role":"assistant","content":"Hi!"},{"role":"user","content":"What's 2+2?"}].

**Q: How does batch processing work?**
Use `create_batch_message` with an array of independent message requests. Each request is processed asynchronously and costs 50% less than individual requests. Use `get_batch_message` to check progress and results. Batches are ideal when you have many unrelated prompts to process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anthropic-alternative](https://vinkius.com/mcp/anthropic-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anthropic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `anthropic-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anthropic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anthropic-alternative": {
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

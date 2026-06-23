# Humanloop (LLM Prompt Management API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/humanloop-llm-prompt-management-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage, version, and deploy LLM prompts directly from your AI agent using the Humanloop API.

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


## Available Tools (12)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Humanloop (LLM Prompt Management API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all prompts in my Humanloop organization."

**🤖 AI Agent:**
> I've retrieved your prompts. You have 3 active prompts: 'customer-support-reply' (ID: pr_1), 'code-refactor-bot' (ID: pr_2), and 'marketing-copy-gen' (ID: pr_3).

---

**👤 You:**
> "Get the details for prompt ID pr_12345."

**🤖 AI Agent:**
> Fetching details for 'pr_12345'... This prompt is named 'Summarizer', using model 'gpt-4', with a template focused on technical documentation. It currently has 5 versions.

---

**👤 You:**
> "Deploy version v_987 of prompt pr_123 to the production environment."

**🤖 AI Agent:**
> Deployment successful. Version 'v_987' of prompt 'pr_123' is now live in the 'production' environment.


## ❓ FAQ

**Q: Can I see the full version history of a specific prompt?**
Yes! Use the `list_prompt_versions` tool with the Prompt ID. It will return all historical versions, allowing you to track changes and metadata over time.

**Q: How do I deploy a prompt version to a specific environment like production?**
You can use the `deploy_prompt` tool. Provide the Prompt ID and the Environment ID to set that specific version as the active deployment for that environment.

**Q: Is it possible to record model outputs for later evaluation?**
Absolutely. Use the `log_to_prompt` tool to record a generation, including the prompt path, messages, and output, which can then be used for evaluation in Humanloop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/humanloop-llm-prompt-management-api](https://vinkius.com/mcp/humanloop-llm-prompt-management-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Humanloop (LLM Prompt Management API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `humanloop-llm-prompt-management-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Humanloop (LLM Prompt Management API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "humanloop-llm-prompt-management-api": {
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

# Eden AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eden-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Equip your AI agent to manage unified AI workflows, track providers, and monitor API usage via the Eden AI platform.

## Description
Integrate **Eden AI**, the unified AI API platform, directly into your AI workflow. Manage your automation workflows and pipelines, track available AI providers (OpenAI, Google, AWS, etc.) across various features, monitor real-time API usage and costs, and oversee your LLM models using natural language.

### What you can do

- **Workflow Oversight** — List and retrieve detailed information and status for all your configured AI automation workflows.
- **Provider Intelligence** — Access the provider registry to monitor available AI capabilities, pricing, and service levels for specific features.
- **Usage Monitoring** — Track real-time API consumption statistics, credit balance, and organizational spending across all providers.
- **Model Management** — List all specific large language models (LLMs) and AI features supported by the Eden AI platform.

### How it works

1. Connect the Eden AI integration to your AI assistant.
2. Authorize using your Eden AI API Key (found in your account settings).
3. Orchestrate your unified AI operations and multi-provider automation through intuitive conversation.

### Who is this for?

- **AI Developers** — Quickly check model availability and feature pricing across providers on the go.
- **Product Managers** — Monitor workflow execution status and API consumption via chat.
- **Operations Teams** — Audit credit balances and organizational usage metadata instantly.


## Available Tools (6)
- **chat_completion**: Specify a provider/model (e.g., openai/gpt-4o) or use @edenai for smart routing.

Generate a chat completion using Eden AI multi-provider routing
- **check_credits**: Check your current Eden AI credit balance
- **list_embedding_models**: List available embedding models on Eden AI
- **monitor_consumption**: Monitor your API consumption and costs over time
- **universal_ai**: Model format: feature/subfeature/provider[/model].

Execute specialized AI tasks (OCR, translation, image generation) via Eden AI
- **create_embedding**: Generate text embeddings via Eden AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eden AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active AI workflows."

**🤖 AI Agent:**
> I've found 5 active workflows, including 'Content Extraction' and 'Multilingual Support Bot'. Would you like to see the configuration steps for Content Extraction?

---

**👤 You:**
> "Show me the pricing for 'sentiment_analysis' across providers."

**🤖 AI Agent:**
> I've retrieved the pricing for sentiment analysis: OpenAI ($0.01 per 1k chars), Google ($0.008 per 1k chars), and AWS ($0.012 per 1k chars). Should I pull the service level metadata for Google?

---

**👤 You:**
> "What is my current Eden AI credit balance?"

**🤖 AI Agent:**
> Your current credit balance is $45.20. Your API usage today has been $1.50 across 3 features. Would you like a breakdown of today's usage by feature?


## ❓ FAQ

**Q: How do I get an Eden AI API Key?**
Log in to your Eden AI account, navigate to **Account Settings** or the **API** section, and you can generate or retrieve your unique API Key from there.

**Q: Does the integration support all AI providers?**
Yes, Eden AI provides a unified interface for many providers. The agent can retrieve availability and pricing for any provider currently supported by the Eden AI platform.

**Q: Can the agent trigger workflow executions?**
This integration currently focuses on listing and auditing workflows, providers, and usage. Triggering new workflow executions should be managed via specific Eden AI API calls or the platform dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eden-ai](https://vinkius.com/mcp/eden-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eden AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eden-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eden AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eden-ai": {
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

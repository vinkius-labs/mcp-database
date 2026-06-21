# Lingyi Wanwu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lingyi-wanwu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Lingyi Wanwu AI models — manage chat completions, embeddings, and monitor Yi model performance directly from any AI agent.

## Description
Connect your AI agents to **Lingyi Wanwu** (01.AI), the high-performance AI lab founded by Dr. Kai-Fu Lee. This MCP provides 10 tools to automate interactions with the Yi series of large language models, including state-of-the-art chat completions, semantic embeddings, and account usage monitoring.

### What you can do

- **Yi Model Interaction** — Trigger chat completions with Yi-34B, Yi-Large, and other optimized models using persistent context
- **Vector Embeddings** — Generate high-dimensional semantic embeddings to power advanced RAG and search workflows
- **Model Intelligence** — List all available models and retrieve granular technical specifications for each version
- **Account Management** — Monitor your token consumption and balance programmatically to optimize costs

### How it works

1. Subscribe to this server
2. Log in to the [**Lingyi Wanwu Developer Platform**](https://platform.lingyiwanwu.com/)
3. Navigate to **API Keys** and generate a new key
4. Identify the model you wish to use (e.g., `yi-large` or `yi-34b-chat-0205`)
5. Insert your **API Key** into the field below to start managing your Yi model workflows.

### Who is this for?

- **AI Developers** — automate the integration of high-performance bilingual (EN/CN) models into custom apps
- **Knowledge Engineers** — build RAG pipelines using Lingyi Wanwu's optimized embedding services
- **System Integrators** — bridge enterprise platforms with the efficient and powerful Yi foundation models


## Available Tools (4)
- **list_models**: List available Yi models
- **chat_completions**: Send a message to a Yi model
- **check_moderation**: Check content for policy violations
- **get_embeddings**: Generate text embeddings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lingyi Wanwu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chat with the Yi-Large model and ask 'Explain the impact of AI on the future of work'."

**🤖 AI Agent:**
> Connecting to Yi engine... Yi-Large responded: 'The impact of AI on work is multi-faceted, ranging from task automation to the creation of new specialized roles...' Would you like me to summarize the key points?

---

**👤 You:**
> "Generate embeddings for my company's mission statement."

**🤖 AI Agent:**
> Retrieving embeddings... I've generated a semantic vector for your mission statement using the Yi-embedding model. The data is now available for your RAG search workflows.

---

**👤 You:**
> "Check my current account balance in Lingyi Wanwu."

**🤖 AI Agent:**
> Checking billing status... Your current account balance is 50.00 CNY. This is sufficient for approximately 2 million tokens on the Yi-Large model.


## ❓ FAQ

**Q: Which Yi model is best for complex reasoning?**
For complex reasoning and high-quality outputs, `yi-large` is recommended. For faster response times and cost efficiency, `yi-medium` or `yi-spark` are excellent alternatives.

**Q: Can I automatically retrieve my remaining account balance?**
Yes! Use the `get_balance` tool. Your agent will connect to the Lingyi Wanwu billing service and return your current remaining credits.

**Q: How do I list all the technical specs for the Yi models?**
Use the `list_models` tool. Your agent will retrieve a list of all models currently available on the platform, along with their IDs and capabilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lingyi-wanwu](https://vinkius.com/mcp/lingyi-wanwu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lingyi Wanwu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lingyi-wanwu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lingyi Wanwu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lingyi-wanwu": {
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

# Anyscale MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anyscale)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Orchestrate your Anyscale infrastructure — manage LLM queries, vectors, services, and cluster batch jobs directly from your AI agent.

## Description
Connect your **Anyscale** environment to your AI agent and manage both AI inference and backend scalable infrastructure natively through natural conversation.

### What you can do

- **Model Discovery and Querying** — List all active foundational models inside your environment and send conversational or zero-shot instruct prompts
- **Embeddings Pipeline** — Generate semantic vector embeddings for arrays of text inputs directly in-flight
- **Services Fleet** — Monitor deployed Ray services, fetch cluster states, and map live service endpoint configurations 
- **Cluster Jobs** — Query Ray batch jobs to inspect recent execution statuses and training metrics right from your terminal

### How it works

1. Subscribe to this server
2. Provide your Anyscale API Key and Base URL
3. Interface with your models, services, and Ray cluster via Claude, Cursor, or your favorite MCP agent

Scale up your AI operations without opening terminal panes to check Ray cluster status.

### Who is this for?

- **AI & MLOps Engineers** — automate the inspection of deployed models, jobs, and embeddings safely during CI workflows
- **Data Scientists** — submit rapid completion tasks to specialized LLMs running inside your Anyscale VPC
- **Backend Developers** — debug service health metrics and endpoint statuses without navigating the heavy cloud dashboard


## Available Tools (7)
- **list_models**: g., meta-llama/Llama-2-70b-chat-hf).

List available AI models on Anyscale Endpoints
- **chat_completion**: Pass an array of messages with roles (user, assistant, system).

Generate conversational responses via Anyscale LLMs
- **text_completion**: Use for foundational instruct generation.

Generate text completion using Anyscale generic completion API
- **generate_embeddings**: Generate semantic vector embeddings for text
- **list_services**: List Anyscale deployed services
- **get_service**: Retrieve details about a specific Anyscale service
- **list_jobs**: List Anyscale batch or training jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anyscale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active models from my Anyscale cluster."

**🤖 AI Agent:**
> I've fetched your models. Currently, you have `meta-llama/Llama-2-70b-chat-hf` and `mistralai/Mistral-7B-Instruct-v0.1` ready to receive inference traffic.

---

**👤 You:**
> "Check the status of our latest training jobs."

**🤖 AI Agent:**
> Looking up recent jobs. The 'daily_retrain_v3' job succeeded 5 hours ago. However, 'experimental_tuning_7b' was interrupted due to out-of-memory errors on node 12. Would you like me to fetch more service metadata on that specific node?

---

**👤 You:**
> "Generate vector embeddings for the text: 'The sun rises in the east and sets in the west'"

**🤖 AI Agent:**
> I've passed the text to your configured Anyscale embedding model. The embedding array generated successfully with 768 dimensions. Since the array is large, I've mapped the output directly to the data pipeline.


## ❓ FAQ

**Q: Can I query a Llama 3 model that is locally deployed in Anyscale?**
Yes. First ask the agent to list the available model APIs using `list_models` so it can grab the precise namespace (e.g. meta-llama/Llama-3-70b-instruct). Then, ask it to run `chat_completion` pointing at that specific ID. You are now effectively chaining your local agent with an enterprise-sized foundational model in your own VPC.

**Q: Is it possible to check whether my training job timed out without opening the Anyscale Dashboard?**
Absolutely. Use the `list_jobs` tool directly from your chat workflow. It will pull down the state of recent tasks (running, failed, succeeded) alongside metrics. The agent can immediately summarize issues if it sees any errors, saving you a context switch.

**Q: Can I use Anyscale to process my text chunks into Vectors inside a project pipeline?**
Yes. This MCP comes with an explicit `generate_embeddings` tool mapped to your Anyscale endpoints. By providing arrays of chunks, the Anyscale fast backbone will return your high-dimensional vectors. Your custom Agent can wrap this into scripts to hydrate vector databases faster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anyscale](https://vinkius.com/mcp/anyscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anyscale** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `anyscale` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anyscale** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anyscale": {
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

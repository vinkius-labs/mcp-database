# TrueFoundry MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truefoundry)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Universal LLM Gateway & ML deployment hub: invoke 1000+ proxy models and manage MCP service instances natively.

## Description
### What you can do

Connect AI agents to TrueFoundry's dual-architecture matrix encompassing both an AI Gateway and a Deployment Orchestrator:

- **Route LLM prompts** securely utilizing a unified endpoint connecting to OpenAI, Anthropic, Gemini, Llama, and more
- **Manage LLM Embeddings** mapping strings flawlessly through secure unified channels
- **Discover Gateway Models** identifying exact runtime limitations and contexts
- **Orchestrate MCP Containers** deploying new AI server topology straight onto infrastructure limits
- **Monitor Active Deployments** generating status, usage array metrics, and isolation limits natively
- **List MCP Schemas** utilizing the managed TrueFoundry MCP discovery engine array
- **Execute Chat streams** dynamically routing user contexts purely bound without touching distinct API keys

### How it works

1. **Generate your TrueFoundry credentials** fetching your Personal Access Token from settings
2. **Identify your dedicated cluster URL** (your exclusive TrueFoundry endpoint domain)
3. **Request inference executions** bounding strictly the proxy routes, completely isolating original vendor APIs from your codebase
4. **Govern deploy processes** natively bypassing complex container matrix orchestrations

### Who is this for?

Essential for **Platform Operations teams**, **AI Engineers**, and **Software Architects** desiring an integrated hub that strips out the N-by-M fragmentation of multiple LLM pipelines and multiple MCP tool servers into a single secure plane.


## Available Tools (8)
- **truefoundry_deploy_mcp_server**: Spawn a new backend container logical process using TrueFoundry service mesh
- **truefoundry_generate_embeddings**: Calculate semantic vectors securely using the unifed abstraction
- **truefoundry_get_deployment_status**: Emit detailed metric states on the orchestration matrix bounds
- **truefoundry_get_mcp_server_info**: Extract exact JSON metadata of one registered TrueFoundry tool schema
- **truefoundry_list_deployments**: Monitor the existing array of running backend topologies mapped to the team
- **truefoundry_list_gateway_models**: List all accessible foundation models from the TrueFoundry unified AI gateway
- **truefoundry_list_mcp_servers**: Extract registry mapping of all available logical MCP Tools in TrueFoundry
- **truefoundry_run_gateway_chat**: g., openai/gpt-4o) mapping the true chat parameter to the gateway.

Perform inference explicitly pushing a model query string through TrueFoundry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TrueFoundry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active AI models supported natively inside my TrueFoundry gateway access instance."

**🤖 AI Agent:**
> Executing `list_gateway_models` cleanly... Extracted dynamic boundaries resolving exactly 23 natively available providers including OpenAI and Cohere. Fetching strict context limits matrix sequentially.

---

**👤 You:**
> "Trigger a chat payload pushing to 'openai-gpt4o' via TrueFoundry querying semantic structures bounding limits."

**🤖 AI Agent:**
> Generating structured call via `run_gateway_chat`. The backend relayed proxy safely isolating original network keys. Response received indicates valid bounding states matching flawlessly.

---

**👤 You:**
> "Deploy the 'supabase-mcp' node-image natively mapping strict variables onto my cluster runtime boundaries."

**🤖 AI Agent:**
> Processing native cluster allocation bounding resources via `deploy_mcp_server`. Configuration schemas synced into TrueFoundry engine cleanly. Running logs verify successful execution state bounds mapped efficiently.


## ❓ FAQ

**Q: Can I route conversational streams directly via the AI agent using the Universal Gateway?**
Yes! You can orchestrate inferences parsing `run_gateway_chat` providing dedicated string formats mapping natively any enabled model.

**Q: Is it possible to monitor crashed services or container states?**
Absolutely. Target the instance ID and emit `get_deployment_status` explicitly bounding execution limits and fetching live log matrices.

**Q: Are the deployment configuration variables isolated upon server launch?**
Yes, using `deploy_mcp_server` dynamically provisions encapsulated boundaries. You stringify environment tokens seamlessly obscuring values into active runtimes only.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truefoundry](https://vinkius.com/mcp/truefoundry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TrueFoundry** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truefoundry` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TrueFoundry** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truefoundry": {
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

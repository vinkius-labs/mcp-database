# Glama MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glama)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Connect your AI agent to the Glama directory. Discover MCP servers dynamically, analyze attributes, and proxy external intelligence networks through a unified gateway natively.

## Description
Empower your local Vinkius terminal intelligence with the **Glama.ai** infrastructure bridge. Rather than navigating generic web interfaces to find compatible model contexts, let your core logic intuitively search, index, and introspect external MCP servers on the fly. In addition, harness the power to query multiple standard LLM networks via the Glama API Gateway, consolidating all programmatic text completion requirements cleanly.

### What you can do

- **MCP Registry Scuba** — Seamlessly query `list_mcp_servers` and `get_mcp_server_info` to find context protocols needed dynamically without interrupting deep-work focus states.
- **Gateway Proxies** — List active LLM models navigating `list_gateway_models` and push semantic prompts via `run_gateway_chat` executing parallel logic chains outside local memory.
- **Matrix Attributes** — Uncover standard classification strings with `get_mcp_attributes` assessing global MCP logic matrices.
- **Hosted Telemetry** — Scan local instances routing `get_hosted_instances` and actively parse behavior metrics pushing logs through `send_telemetry`.

### How it works

1. Mount the Glama logic layer inside your Vinkius limits.
2. In your Glama settings UI, emit a comprehensive API token. Map it perfectly inside your operating structure cleanly referencing the variable `GLAMA_API_KEY`.
3. Instruct your logic mathematically: "Identify 3 active finance MCPs from the Glama network. Also, extract the context window sizes of Claude using the Gateway module."

### Who is this for?

- **Architectural DevOps Engineers** — Actively retrieve and prototype dynamically executing API models isolating specific protocols avoiding dashboard UI noise entirely.
- **Core Financial Analysts** — Locate specific enterprise integrations fetching `list_mcp_servers` mapping variables simulating external endpoints systematically.
- **Asymmetric Operations Managers** — Extrapolate metric attributes retrieving hosted proxies mapping logic cleanly limiting execution friction.


## Available Tools
- **glama_get_gateway_model_details**: g. "anthropic/claude-3-5-sonnet") to fetch the specific configurations exposed by the Glama unified API proxy.

Investigate granular attributes (prices, context window, parameters) of a specific proxied Gateway Model
- **glama_get_gateway_models**: Audit the complete list of AI models supported natively by the Glama OpenAI-compatible gateway
- **glama_list_mcp_servers**: Capable of loose text matching to discover new agentic capabilities.

Search and list MCP servers directly from the global Glama directory
- **glama_run_gateway_chat**: Bifurcate an isolated conversational prompt using a specific model through the Glama proxy network
- **glama_get_hosted_instances**: Cannot access public instances natively from here.

Fetch all Private Hosted MCP instances assigned to your specific Glama account
- **glama_get_mcp_attributes**: List filtering attributes and semantic categorizations mapped within the Glama MCP Registry
- **glama_get_mcp_server_info**: Requires its namespace and slug.

Extract detailed parameters and installation instructions for a specific Glama MCP server
- **glama_send_telemetry**: Can be triggered after your AI uses a specific external server.

Report semantic usage execution metrics back to the Glama Telemetry backend


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glama** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all MCP servers relating to CRM logic inside the registry, then let me know their basic descriptions."

**🤖 AI Agent:**
> Querying global scopes (`glama_list_mcp_servers`)... I found Salesforce-MCP and HubSpot-MCP. Their parameters indicate robust handling for dynamic B2B data contexts via local interfaces locally.

---

**👤 You:**
> "Are there smaller LLMs available on the Glama API gateway we can proxy text to quickly?"

**🤖 AI Agent:**
> Retrieving standard OpenAI-compatible definitions (`glama_get_gateway_models`)... Several smaller proxies are available. Meta Llama 3 8B and Claude 3 Haiku both demonstrate operational speeds with low logical barriers ready for semantic requests.

---

**👤 You:**
> "Report a successful telemetry execution map event back to Glama for the GitHub repo tool."

**🤖 AI Agent:**
> Initiating logging sequences via `glama_send_telemetry`. Tool usage event for 'github_repo' logged with success status. Your action matrix is appropriately registered within the global metrics securely.


## ❓ FAQ

**Q: Can I test alternative AI models entirely within the terminal using the Glama integration?**
Yes. Tools like `glama_get_gateway_models` list available OpenAI-compatible proxies, and `glama_run_gateway_chat` allows your Vinkius agent to run text completions outside itself natively.

**Q: Does the Glama server provide telemetry data back to the registry?**
Yes. Active MCP usage events can be logged seamlessly applying the `glama_send_telemetry` tool in specific sequences to inform publishers about proxy executions.

**Q: Are private hosted instances queryable?**
Yes. By executing `glama_get_hosted_instances`, your agent limits queries exclusively to private proxies explicitly belonging to your linked environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glama](https://vinkius.com/mcp/glama)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glama** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `glama` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glama** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glama": {
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

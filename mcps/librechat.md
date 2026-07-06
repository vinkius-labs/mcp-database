# LibreChat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/librechat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate your LibreChat instance — manage agents, list available models, and generate AI completions via the Agents and Open Responses APIs.

## Description
Connect your **LibreChat** instance to any AI agent and gain programmatic control over your self-hosted AI ecosystem. This server allows you to bridge your custom agents and models with any MCP-compatible client.

### What you can do

- **Agent Orchestration** — List all available agents and models configured in your LibreChat environment.
- **Unified Completions** — Create chat completions using the Agents API, providing an OpenAI-compatible interface for your custom setups.
- **Open Responses** — Utilize the Open Responses API specification to generate structured AI outputs.
- **Session Management** — Authenticate directly via email and password to retrieve access tokens when a static API key is not preferred.

### How it works

1. Subscribe to this server
2. Provide your LibreChat Base URL and API Key (or use the login tool)
3. Start interacting with your private LLM agents through Claude, Cursor, or other MCP tools.

### Who is this for?

- **AI Engineers** — integrate self-hosted LibreChat agents into automated workflows and IDEs.
- **DevOps Teams** — monitor and query available model configurations across different environments.
- **Power Users** — centralize access to multiple private LLMs through a single, secure interface.


## Available Tools (4)
- **open_responses**: Create a response using the Open Responses API
- **chat_completions**: Model corresponds to an Agent ID.

Create a chat completion using the Agents API
- **list_models**: List available LibreChat models/agents
- **login**: Login to LibreChat to get access and refresh tokens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LibreChat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available agents in my LibreChat instance."

**🤖 AI Agent:**
> I've retrieved the available agents. You have access to: 'Research-Assistant' (ID: agent_123), 'Code-Interpreter' (ID: agent_456), and 'General-Chat' (ID: agent_789).

---

**👤 You:**
> "Login to LibreChat using my credentials."

**🤖 AI Agent:**
> Authentication successful. I have obtained the access and refresh tokens for your session. You can now proceed with querying models or creating completions.

---

**👤 You:**
> "Ask agent_123 to summarize the latest trends in AI."

**🤖 AI Agent:**
> Sending request to agent_123... The agent responded: 'The current trends in AI include the rise of multi-modal models, autonomous agentic workflows, and increased focus on efficient small language models (SLMs)...'


## ❓ FAQ

**Q: How can I see which agents are currently available in my LibreChat instance?**
You can use the `list_models` tool. It will query your configured LibreChat instance and return a list of all accessible agents and models associated with your credentials.

**Q: Can I use this server to chat with a specific agent by its ID?**
Yes! Use the `chat_completions` tool. Simply provide the `model` (which is the Agent ID) and an array of `messages` to generate a response from that specific agent.

**Q: What should I do if I don't have a static API key for my instance?**
You can use the `login` tool. By providing your email and password, the server will authenticate with LibreChat and retrieve the necessary access tokens for subsequent requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/librechat](https://vinkius.com/mcp/librechat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LibreChat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `librechat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LibreChat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "librechat": {
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

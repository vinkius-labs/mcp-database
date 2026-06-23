# AutoGen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autogen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Orchestrate Microsoft AutoGen multi-agent workflows — manage sessions, agent roles, workflows, and monitor execution logs from any AI agent.

## Description
Connect your **AutoGen Studio** instance to any AI agent and take full control of your multi-agent topologies and execution memory spaces through natural conversation.

### What you can do

- **Sessions** — Create and manage blank, isolated memory spaces for your multi-agent workflows to run cleanly
- **Messages** — Dispatch human prompts and retrieve deep agent-to-agent conversational traces inside Microsoft's logging structures
- **Agents** — Map out and dynamically define customized LLM roles (User_Proxy, Coder, Critic) using Python-based parameters
- **Workflows & Skills** — Visualize routing topographies, available graph deployments, and injected native Python capabilities
- **Models** — Audit existing constrained fallback OpenAI configurations natively stored in the engine

### How it works

1. Subscribe to this server
2. Provide your AutoGen Studio instance Base URL
3. Start dispatching nested groups of AI agents directly from Claude, Cursor, or any MCP-compatible client

Your primary agent can now command and debug secondary swarms of specialized agents dynamically.

### Who is this for?

- **AI Engineers** — audit running agent topologies, trace deep execution logs, and iterate on Python skills without swapping contexts
- **Product Managers** — verify the health and steps of automated backend swarm operations
- **Researchers** — easily extract deep LLM-to-LLM conversational histories across experimental boundaries for grading


## Available Tools (10)
- **create_agent**: Define a new customized AutoGen agent
- **create_message**: Send a user message to initiate or continue an AutoGen session
- **list_skills**: List Python skill functions available to AutoGen agents
- **create_session**: Create a new blank AutoGen session
- **delete_session**: Permanently delete an AutoGen session
- **list_agents**: List all configured AutoGen agents available
- **list_messages**: Retrieve the message history for a specific AutoGen session
- **list_models**: List Large Language Models configured for use in AutoGen
- **list_sessions**: List AutoGen Studio conversation sessions
- **list_workflows**: List all predefined AutoGen multi-agent workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AutoGen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all configured LLM models available right now."

**🤖 AI Agent:**
> You have 3 restricted LLM configurations available in your AutoGen Studio instance. gpt-4-turbo for complex agents, gpt-3.5-turbo mapped for basic coder roles, and a local quantized llama-3 constraint. Want me to inspect the multi-agent Workflows built on top of them?

---

**👤 You:**
> "Analyze the message traces for the session running the Code Reviewer."

**🤖 AI Agent:**
> Fetching historical agent-to-agent traces for Tracker UUID cd82-... User_Proxy provided the diff 3 minutes ago. Coder_Agent built a solution, but Critic_Agent heavily rejected it due to a hard-coded API key security issue inside the script. The Coder is currently stalled retrying a new commit implementation. Should I intervene?

---

**👤 You:**
> "Create a new isolated session and execute the research workflow."

**🤖 AI Agent:**
> A new clean boundary UUID a9f2-bcd has been created. I've successfully routed a POST Message into it targeting the 'Market Research' topograph topology. The agentic group is starting now. Should I poll it and summarize their conclusions after five minutes?


## ❓ FAQ

**Q: Can my AI agent debug a looping multi-agent conversation?**
Yes. You can instruct your primary agent to retrieve the message traces for a specific AutoGen session ID. It will instantly unpack the internal LLM-to-LLM conversation, highlighting exactly which secondary agent is looping, throwing errors, or deviating from the constraints without manual log parsing.

**Q: How do I add a new Python capability or skill dynamicly?**
Your agent can list currently mapped Python skills bound to the studio runtime. If you need a new capability, your primary AI can iterate on the script directly on your CLI/editor and once deployed in your studio, you can map it natively to customized agents via the creation parameters.

**Q: Can it trigger a Workflow to start executing a new complex task?**
Absolutely. Ask your agent to create a fresh, blank, and completely isolated session, then dispatch a newly constructed 'human message' targeting an existing Multi-Agent workflow topology. It initiates the whole automated logic sequence securely and remotely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autogen](https://vinkius.com/mcp/autogen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AutoGen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `autogen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AutoGen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autogen": {
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

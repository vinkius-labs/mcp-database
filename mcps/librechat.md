# LibreChat MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/librechat)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/librechat-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/librechat-mcp)
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


## Available Tools
- **chat_completions**: Model corresponds to an Agent ID.

Create a chat completion using the Agents API
- **list_models**: List available LibreChat models/agents
- **login**: Login to LibreChat to get access and refresh tokens
- **open_responses**: Create a response using the Open Responses API


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


## Installation & Usage

To install and use the **LibreChat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/librechat](https://vinkius.com/mcp/librechat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

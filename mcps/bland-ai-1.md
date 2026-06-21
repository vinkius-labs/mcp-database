# Bland AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bland-ai-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bland-ai-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bland-ai-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Automate phone calls via Bland AI — send outbound calls, manage agents, and retrieve transcripts directly from any AI agent.

## Description
Connect your **Bland AI** account to any AI agent and orchestrate your automated phone call workflows through natural conversation.

### What you can do

- **Outbound Automation** — Send AI-powered phone calls with custom tasks and specific voices.
- **Call Monitoring** — List recent calls and retrieve detailed metadata, including transcripts and analysis.
- **Agent Management** — Access and manage your AI 'personas' (agents) used for different call scenarios.
- **Pathway Coordination** — Retrieve and utilize complex conversation pathways for branching logic during calls.
- **Voice Discovery** — List all available AI voices to find the perfect fit for your brand.
- **Operational Control** — Stop active or scheduled calls instantly if needed.

### How it works

1. Subscribe to this server
2. Enter your Bland AI API Key
3. Start automating your phone operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Support Teams** — automate follow-ups and appointment reminders without manual dialing.
- **Operations Leads** — monitor call performance and agent settings straight from their workflow tools.
- **Developers** — integrate automated phone interactions into their agent-led business processes.


## Available Tools
- **get_agent**: Get details of a specific AI agent
- **get_call**: Get details and metadata of a call
- **get_pathway**: Get details of a specific pathway
- **get_transcript**: Retrieve the transcript of a completed call
- **list_agents**: List all AI agents
- **list_calls**: List recent AI calls
- **list_pathways**: List all conversation pathways
- **list_voices**: List available AI voices
- **send_call**: Send an AI phone call
- **stop_call**: Stop an active or scheduled call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bland AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Call +15550199 and ask if they are still interested in our pricing plan."

**🤖 AI Agent:**
> I've initiated the call to +15550199. Call ID is 'call_123'. I've instructed the AI to inquire about pricing interest. You can check the status or transcript once it's finished.

---

**👤 You:**
> "List all AI agents in my account."

**🤖 AI Agent:**
> I've retrieved your agents. You have 'Sales Assistant' (ID: agent_1), 'Support Bot' (ID: agent_2), and 'Lead Qualifier' (ID: agent_3).

---

**👤 You:**
> "Show the transcript for call call_998877."

**🤖 AI Agent:**
> Retrieving transcript... Here is the conversation log: [AI]: 'Hello, I'm calling from Acme...' [Customer]: 'Yes, tell me more about...' Would you like an analysis of this call?


## Installation & Usage

To install and use the **Bland AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bland-ai-1](https://vinkius.com/mcp/bland-ai-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

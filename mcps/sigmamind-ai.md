# SigmaMind AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sigmamind-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sigmamind-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sigmamind-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Train custom computer vision models with your own images and deploy object detection and classification without ML expertise.

## Description
Connect your **SigmaMind** account to any AI agent and manage AI voice workflows.

### What you can do

- **Call Management** — List calls, initiate new calls, and check status
- **Agent Configuration** — Create and inspect AI voice agents with custom prompts
- **Transcript Access** — Retrieve full conversation transcripts for completed calls
- **Call Analysis** — Get AI-generated sentiment and topic analysis
- **Phone Numbers** — View assigned phone numbers
- **Health Check** — Verify API connectivity


## Available Tools
- **check_sigmamind_status**: Verify API connectivity
- **create_agent**: Create a voice agent
- **create_call**: Initiate a voice call
- **get_agent**: Get agent details
- **get_call_analysis**: Get call analysis
- **get_call**: Get call details
- **get_call_transcript**: Get call transcript
- **list_agents**: List all agents
- **list_calls**: List all calls
- **list_numbers**: List phone numbers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SigmaMind AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AI voice agents."

**🤖 AI Agent:**
> You have 3 agents: 'Sales Qualifier' (42 calls), 'Support Bot' (128 calls), 'Survey Agent' (15 calls).

---

**👤 You:**
> "Call +14155551234 with agent 'Sales Qualifier'."

**🤖 AI Agent:**
> Call initiated! ID: call_8291 to +14155551234 using 'Sales Qualifier'. The AI agent is now handling the conversation.

---

**👤 You:**
> "Show transcript for call call_8291."

**🤖 AI Agent:**
> Transcript for call_8291 (3m 42s): Agent greeted the contact, qualified interest in the product, and scheduled a demo for next Tuesday.


## Installation & Usage

To install and use the **SigmaMind AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sigmamind-ai](https://vinkius.com/mcp/sigmamind-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

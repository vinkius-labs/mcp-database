# Bland AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bland-ai-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bland-ai-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bland-ai-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Deploy AI phone agents that handle inbound and outbound calls with natural conversation for sales and customer support.

## Description
Connect your **Bland AI** account to any AI agent and take full control of your hyper-realistic AI-driven phone communication and automated voice workflows through natural conversation.

### What you can do

- **Outbound Call Orchestration** — Programmatically initiate high-fidelity phone calls to over 200 countries, providing specific tasks and real-time instructions directly through your agent
- **Voice Agent Architecture** — Create and manage persistent AI personas with fixed prompts, voices, and personality settings to maintain a perfectly coordinated brand voice
- **Conversation Intelligence** — Access real-time call statuses, retrieve complete high-fidelity transcripts, and access secure recording links for every interaction
- **Post-Call Discovery** — Programmatically analyze finished calls to extract specific variables, insights, or sentiment summaries using advanced post-processing tools
- **Infrastructure Monitoring** — Access your directory of purchased phone numbers and high-fidelity AI voices to oversee your voice communication ecosystem programmatically

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Bland AI dashboard (Settings > API Keys)
3. Start orchestrating your automated voice outreach from Claude, Cursor, or any MCP client

No more manual dialing or listening through hours of recordings to find insights. Your AI acts as your dedicated telephony engineer and voice interaction coordinator.

### Who is this for?

- **Sales & Operations Leads** — instantly initiate lead qualification calls and monitor conversion trends using natural language commands
- **Customer Success Managers** — automate appointment reminders and analyze customer sentiment without leaving your workspace
- **Developers** — integrate high-speed AI voice interactions into custom business workflows through simple AI queries


## Available Tools
- **analyze_call_transcript**: Perform post-call analysis
- **stop_active_call**: Stop an ongoing phone call
- **create_voice_agent**: Create a persistent AI persona
- **delete_voice_agent**: Remove an AI persona
- **get_agent_config**: Get agent settings
- **get_call_details**: Get details and transcript for a call
- **list_voice_agents**: List configured AI personas
- **list_recent_calls**: List recent phone calls
- **list_phone_numbers**: List purchased phone numbers
- **list_available_voices**: List high-fidelity AI voices
- **send_phone_call**: Send an outbound phone call using an AI agent
- **update_agent_config**: Modify agent settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bland AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Call '+15551234567' and ask if they are still coming to the meeting today at 3 PM."

**🤖 AI Agent:**
> Call initiated! I've successfully triggered an outbound call via Bland AI to +15551234567. The agent is instructed to verify the 3 PM meeting. Shall I alert you when the transcript is ready?

---

**👤 You:**
> "Show the transcript and recording for call ID 'call_123'."

**🤖 AI Agent:**
> Fetching call data... I've retrieved the transcript for call_123. The recipient confirmed they are coming. You can access the high-fidelity recording here: [url]. Need any help with post-call analysis?

---

**👤 You:**
> "List all my persistent voice agents in Bland AI."

**🤖 AI Agent:**
> Accessing voice personas... You currently have 3 configured agents, including 'Support Maya' (Voice: Maya) and 'Sales Mason'. Would you like the detailed prompt configuration for any of them?


## Installation & Usage

To install and use the **Bland AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bland-ai-alternative](https://vinkius.com/mcp/bland-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

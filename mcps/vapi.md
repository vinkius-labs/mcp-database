# Vapi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Command Voice AI assistants directly from your chat. Make outbound phone calls, update personas, and retrieve full transcripts via Vapi.

## Description
Connect your **Vapi** account to any AI agent and bring the power of automated voice communication into your standard conversational workspace.

### What you can do

- **Phone Calling** — Send commands instructing the agent to place outbound human-like phone calls and establish web ringing connections through Vapi's PSTN/WebRTC capabilities.
- **Call Transcripts** — Search through recent call logs, retrieve call details natively, and pull raw voice-to-text transcripts or conversation metrics.
- **Persona Engineering** — Ask your chat agent to build new Vapi assistants, update their system prompts, change its specific model, or mutate Voice IDs on the fly.
- **Squad Routing** — List available telephony numbers, tools, and multi-agent squads natively to configure advanced conversational pathways.

### How it works

1. Subscribe to this server
2. Enter your Vapi Private API Key
3. Start initiating and tracking phone calls from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a robust telephony dispatch center.

### Who is this for?

- **Sales Engineers** — quickly tell the agent to place a demonstration outbound sales call to a prospect's number right from your editor.
- **Customer Support Teams** — pull the exact voice transcript logic from an unhappy customer call to summarize action items instantaneously.
- **Voice AI Developers** — tweak TTS voices, change LLM models, or rewrite system instructions for a new assistant iteratively without switching windows.
- **Operations Managers** — rapidly audit active telephony numbers and connected toolsets across different Vapi environments.


## Available Tools
- **create_assistant**: Provide configuration for transcriber, model, and voice as a JSON string.

Create a new Voice AI assistant persona
- **create_phone_call**: Provide the phone number ID and customer details.

Start a new outbound phone call via Vapi
- **create_web_call**: Returns a web call configuration.

Generate a new web-based voice call link
- **get_call_details**: Retrieves details, transcripts, and metrics for a specific call
- **list_assistants**: List all Voice AI assistants configured in Vapi
- **list_calls**: List recent and active voice calls managed by Vapi
- **list_phone_numbers**: List all phone numbers connected to Vapi
- **list_squads**: List all multi-agent squads
- **list_agent_tools**: List all tools available to Vapi assistants
- **update_assistant**: Update an existing assistant configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vapi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our configured Voice assistants and their IDs."

**🤖 AI Agent:**
> You currently have 3 conversational Voice AI assistants configured in Vapi: 'Lead Qualification Bot' (ID: ba1-342x), 'Support Intake Matrix' (ID: cd3-99ab), and 'Internal Switchboard' (ID: 9fz-77qp). Do you want to see the system prompts behind any of these?

---

**👤 You:**
> "Get the details and full transcript for call ID 'vapi1234'."

**🤖 AI Agent:**
> I've retrieved the call log for 'vapi1234'. This was an outbound call that lasted 2 minutes and 15 seconds. 

**Summary:** The AI Assistant contacted John Doe about his recent warranty claim. John indicated he has already shipped the defective unit. The AI processed this information gracefully and closed the ticket conceptually.

Here is a snippet of the transcript:
*User:* 'Yeah I sent it out through FedEx yesterday.'
*Assistant:* 'Perfect, thank you John! I have updated your claim status to incoming...'

---

**👤 You:**
> "Update assistant 'Bot Support' to change its `model.model` parameter to `gpt-4o-mini`."

**🤖 AI Agent:**
> Successfully updated the conversational model for 'Bot Support'. It has transitioned in Vapi engine logic and is now utilizing `gpt-4o-mini`. Its next active conversation will run purely on this adjusted backend structure.


## Installation & Usage

To install and use the **Vapi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vapi](https://vinkius.com/mcp/vapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

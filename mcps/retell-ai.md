# Retell AI MCP Server

Empower your conversational AI to orchestrate, analyze, and automate phone calls or web-based voice agent interactions via Retell.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/retell-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
Connect your conversational assistant directly to **Retell AI**, a powerful platform for building voice-driven conversational agents. Empower your AI to orchestrate, analyze, and automate phone calls or web-based voice interactions seamlessly via simple text commands. From provisioning intelligent voice agents to placing outbound calls to customers, this integration brings the full telecommunication stack directly to your chat interface.

### What you can do

- **Automate Phone Calls** — Command your assistant to initiate outbound voice interactions on your behalf (`create_phone_call`) or register active sessions for web browser integration (`register_web_call`).
- **Build and Manage Voice Agents** — Dynamically orchestrate AI agent personalities (`create_agent`, `update_agent`) and configure their underlying conversational brain (`create_llm`) with specific system instructions and models.
- **Analyze Telemetry** — Keep track of your infrastructure by querying historical call logs (`list_calls`), investigating specific conversations for transcripts and sentiment analysis (`get_call_details`), surveying available text-to-speech voices (`list_voices`), and reviewing provisioned communication lines (`list_phone_numbers` and `list_agents`).

### How it works

1. Install the Retell extension module within your MCP environment.
2. Obtain your `Retell API Key` from your official provider account and securely input it into the designated authentication parameter below.
3. Simply chat with your assistant: "Review all my available voices, create a new AI voice agent configured as a customer support representative, and initiate a test phone call to my personal number."

### Who is this for?

- **Founders & Operators** — Spin up autonomous voice-driven receptionists or support bots to interact with inbound or outbound telecommunication traffic efficiently.
- **Developers & Integrators** — Manage Retell AI configurations and rapidly prototype voice applications without using Postman or coding custom administration panels.
- **Workflow Orchestrators** — Chain natural language instructions to dynamically assess previous call transcripts and adjust an active agent's system prompt accordingly.


## Available Tools
- **create_agent**: Creates a new AI voice agent
- **create_llm**: Configures a Retell-hosted LLM
- **create_phone_call**: Provide a JSON payload with "from_number" and "to_number".

Initiates an outbound phone call
- **get_call_details**: Retrieves details for a specific call
- **list_agents**: Lists all configured AI voice agents
- **list_calls**: Lists all historical and active calls
- **list_phone_numbers**: Lists all phone numbers associated with the account
- **list_voices**: Lists all available text-to-speech voices
- **register_web_call**: Registers a new web-based call
- **update_agent**: Updates an existing AI voice agent


## Installation & Usage

To install and use the **Retell AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retell-ai](https://vinkius.com/mcp/retell-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

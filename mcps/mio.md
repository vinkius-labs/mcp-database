# Mio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Bridge conversations between Slack, Microsoft Teams, and Webex so teams on different platforms can collaborate without switching apps.

## Description
Connect your **Mio** account to any AI agent and manage automated phone calls through natural conversation.

### What you can do

- **Outbound Calls** — Start AI-powered phone calls with custom scripts and instructions
- **Call Logs** — Browse call history with status, duration, and outcomes
- **Transcripts** — Retrieve full text transcriptions of completed calls
- **AI Summaries** — Get AI-generated summaries and extracted data from calls
- **Voice Selection** — Choose from multiple neural voices for the AI agent
- **Webhooks** — Configure event notifications for call status changes
- **Call Control** — Terminate active calls in real time
- **Account** — Check credit balance and account information

### How it works

1. Subscribe to this server
2. Enter your Mio API Key
3. Start making AI calls from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — automate outbound prospecting calls with AI agents
- **Customer Service** — deploy AI voice agents for appointment confirmations
- **Developers** — build voice-first AI applications with call transcripts


## Available Tools
- **start_ai_call**: Start an AI phone call
- **create_webhook**: Add new notification
- **delete_webhook**: Remove a webhook
- **get_account_info**: Get user profile
- **get_call_details**: Get specific call info
- **get_credit_balance**: Check account funds
- **get_call_summary**: Get AI call summary
- **get_call_transcript**: Get call text log
- **list_calls**: List all call logs
- **list_available_voices**: List AI voices
- **list_webhooks**: Get active webhooks
- **terminate_call**: Stop active call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start an AI call to confirm tomorrow's appointment with Sarah."

**🤖 AI Agent:**
> AI call started! ✅ Call ID: call_890. Number: +1-555-0123. Instructions: 'Confirm tomorrow's appointment at 10 AM. Ask if the time still works. Be polite and professional.' Voice: Maya. Status: Ringing...

---

**👤 You:**
> "Get the transcript and summary for call_890."

**🤖 AI Agent:**
> Call call_890 completed (Duration: 1m 45s). Transcript: AI: 'Hi Sarah, I'm calling to confirm your appointment tomorrow at 10 AM.' Sarah: 'Yes, that works perfectly.' AI: 'Great, see you then!' Summary: Appointment confirmed for tomorrow 10 AM. Outcome: Positive. No reschedule needed.

---

**👤 You:**
> "Show available AI voices and my credit balance."

**🤖 AI Agent:**
> Available voices: 6. 'Maya' (Female, US English, Warm). 'Alex' (Male, US English, Professional). 'Luna' (Female, British). 'Marco' (Male, Spanish). 'Sophie' (Female, French). 'Kai' (Male, US English, Casual). Credits remaining: $42.50 (approx. 85 minutes of calls).


## Installation & Usage

To install and use the **Mio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mio](https://vinkius.com/mcp/mio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

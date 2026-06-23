# Vapi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vapi)
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


## Available Tools (10)
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


## ❓ FAQ

**Q: Can the agent place an outbound phone call for me?**
Yes! Through the `createPhoneCallTool`, you can ask your agent: `Initiate a phone call to +15551234567 using our 'Sales Assistant' persona`. It will format the payload correctly and instruct Vapi to dial the human using the specified AI persona.

**Q: How can I read the transcript of an old automated voice call?**
Just tell your chat assistant: `fetch the transcript details for call ID '3fbea5x...'`. The `getCallTool` reaches into Vapi, extracts the raw audio-to-text transcript logs, and the assistant can even summarize the entire human-to-AI interaction for you.

**Q: Can I tweak system prompts or models sequentially in my chat editor?**
Yes, especially if you're in an IDE like Cursor. You can iterate: `Update Assistant 'Agent A' to use GPT-4o and set its prompt to 'Always be highly overly enthusiastic'`. The agent will use the `updateAssistantTool` to reconfigure the live voice persona instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vapi](https://vinkius.com/mcp/vapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vapi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vapi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vapi": {
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

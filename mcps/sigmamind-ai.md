# SigmaMind AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sigmamind-ai)
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


## ❓ FAQ

**Q: Can my AI initiate phone calls?**
Yes. Use `create_call` with an agent ID and phone number. The AI agent handles the conversation automatically.

**Q: Can I read call transcripts?**
Yes. `get_call_transcript` returns the full conversation for any completed call.

**Q: How do I create a new voice agent?**
Use `create_agent` with a name and system prompt. The agent will use the prompt to guide conversations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sigmamind-ai](https://vinkius.com/mcp/sigmamind-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SigmaMind AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sigmamind-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SigmaMind AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sigmamind-ai": {
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

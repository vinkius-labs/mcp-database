# Retell AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retell-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build human-like AI voice agents that handle phone calls, answer questions, and complete tasks through natural spoken conversation.

## Description
Connect your **Retell AI** account to any AI agent and take full control of your conversational voice orchestration through natural conversation. Retell AI provides a premier platform for building human-like voice agents, and this integration allows you to create agents, initiate phone or web calls, and monitor LLM configurations directly from your chat interface.

### What you can do

- **Agent & Persona Orchestration** — List all managed voice agents and retrieve detailed persona metadata, including creating new agents programmatically.
- **Call Lifecycle Management** — Initiate and monitor real-time phone or web calls and retrieve detailed call metadata including recordings and transcripts directly from the AI interface.
- **LLM & Brain Control** — Access and monitor your Retell LLM configurations to ensure your agents always have the correct logic and knowledge via natural language.
- **Phone Number Intelligence** — List available phone numbers to maintain a clear overview of your telephony infrastructure.
- **Operational Monitoring** — Track system responses and manage agent settings using simple AI commands to ensure your voice operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Retell AI API Key from your dashboard settings
3. Start managing your voice agents from Claude, Cursor, or any MCP-compatible client

No more manual call logs or complex agent configuration. Your AI acts as a dedicated voice operations manager or AI lead.

### Who is this for?

- **AI Developers & Product Managers** — quickly retrieve call details and monitor agent performance without switching apps.
- **Customer Support Operations** — automate the management of voice personas and track call history via natural conversation.
- **Operations Teams** — streamline the retrieval of agent metadata and monitor organizational voice health directly within the chat.


## Available Tools
- **get_phone_number**: Get details for a specific phone number
- **create_voice_agent**: Create a new AI voice agent
- **start_phone_call**: Initiate an outbound phone call
- **start_web_call**: Initialize a browser-based call
- **get_agent_config**: Get details for a voice agent
- **get_call_details**: Get details and transcript for a call
- **get_llm_details**: Get metadata for a response engine
- **list_voice_agents**: List all AI voice agents
- **list_recent_calls**: List call logs and history
- **list_retell_llms**: List internal response engines
- **list_retell_numbers**: List registered phone numbers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retell AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my voice agents in Retell AI."

**🤖 AI Agent:**
> I've retrieved your agents. You have 3 active personas: 'Customer Support Cimo', 'Sales Assistant', and 'Outbound Lead'. Which one would you like to update?

---

**👤 You:**
> "Show me all AI voice agents and their call statistics from the last 7 days."

**🤖 AI Agent:**
> 4 active voice agents. "Sales Qualifier" handled 234 calls (avg duration: 3.2 min, 67% qualified leads, 89% caller satisfaction). "Support Assistant" took 567 calls (avg 4.1 min, 78% resolved without transfer, 92% satisfaction). "Appointment Scheduler" booked 145 appointments from 189 calls (76.7% booking rate). "Survey Collector" completed 89 surveys from 120 calls (74.2% completion). Total calls: 1,010. Total minutes: 3,434. Average latency: 0.8 seconds.

---

**👤 You:**
> "Create a new outbound phone call using the Sales Qualifier agent to contact a prospect."

**🤖 AI Agent:**
> Outbound call initiated. Agent: Sales Qualifier (ID: agent_4521). Phone number: +1-555-0234 (from your verified number pool). Calling: +1-555-0198 (prospect: David Chen, ScaleUp Inc). Call script: Lead qualification with product demo scheduling. Call status: Ringing... Connected at 0:03. Agent is conducting the qualification flow. Live transcript available in dashboard. Expected duration: 3-5 minutes. Recording: enabled. Post-call webhook configured for CRM sync.


## ❓ FAQ

**Q: Can my AI automatically create a new phone call to a customer using a specific agent?**
Yes! Use the `create_phone_call` tool. Provide the destination phone number and the `agent_id`, and your agent will trigger the outbound AI voice call instantly.

**Q: How do I list all my available Retell voice agents?**
Simply ask the agent to run the `list_agents` action. It will retrieve the full catalog of voice agents configured in your Retell AI account.

**Q: How do I find my Retell AI API Key?**
Log in to your Retell AI dashboard, navigate to **Settings** > **API Keys**, and you will find your unique secret API key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retell-ai-alternative](https://vinkius.com/mcp/retell-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retell AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `retell-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retell AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retell-ai-alternative": {
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

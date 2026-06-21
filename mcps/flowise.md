# Flowise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage low-code AI workflows via Flowise — run predictions, track chatflows and agentflows, handle tools, and audit execution history directly from any AI agent.

## Description
Connect your **FlowiseAI** instance to any AI agent and take full control of your low-code generative AI application development through natural conversation.

### What you can do

- **Chatflow Orchestration** — List and retrieve detailed architectural nodes and edges for all deployed Chatflows within your Flowise instance natively
- **Agentic Workflow Control** — Access compound Agentflows defining complex AI tasks and multi-step reasoning logic synchronously
- **Live AI Prediction** — Commands the backend to submit user questions to specific Chatflows and retrieve generated AI responses in real-time
- **Execution History Auditing** — Pull precise past execution traces and conversational logs to debug logic chains and monitor agent performance limitlessly
- **Tool & Integration Discovery** — Retrieve custom tools and third-party integrations configured in your Flowise environment to verify available capabilities
- **Credential Oversight** — Enumerate stored credential components used to authenticate your AI logic chains securely within the platform
- **System Health Monitoring** — Verify instance status and available base endpoints to ensure your AI orchestration layer is operational

### How it works

1. Subscribe to this server
2. Enter your Flowise Base URL and API Key (found in your Flowise Settings)
3. Start managing your AI workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug Chatflows and Agentflows without leaving the development environment
- **Automation Engineers** — trigger AI predictions and monitor execution histories using natural language
- **Product Teams** — audit available AI tools and verify conversational logs in real-time
- **Data Scientists** — evaluate different LLM orchestration patterns and logic chains through natural conversation


## Available Tools
- **list_chatflows**: List chatflows
- **get_chatflow**: Get chatflow details
- **predict**: Run prediction on chatflow
- **list_agentflows**: List agentflows
- **list_tools**: List available tools
- **list_credentials**: List credentials
- **get_history**: Get chat execution history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flowise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask chatflow 'abc-123': 'Summarize this document: [Context]'"

**🤖 AI Agent:**
> Prediction initiated! I've sent your request to Flowise chatflow abc-123. The AI response is: 'Based on the provided context, the document outlines three primary growth strategies for the next fiscal year...'

---

**👤 You:**
> "List all active chatflows in my instance"

**🤖 AI Agent:**
> Retrieving chatflows... I found 5 active flows: 'Customer Support Bot', 'RAG Knowledge Base', 'Legal Assistant', 'Lead Generator', and 'Developer Helper'. Which one would you like to explore?

---

**👤 You:**
> "Show me the execution history for chatflow 'Legal-Assistant'"

**🤖 AI Agent:**
> Retrieving history... For 'Legal-Assistant' (ID: 789), I found 10 recent executions. Highlights include a query about 'GDPR compliance' and another regarding 'Contract Review'. Would you like the logs for any of these?


## ❓ FAQ

**Q: Can my agent run a prediction against a specific Flowise chatflow?**
Yes. Use the 'predict' tool. Provide the 'chatflow_id' and your question. The agent will command the Flowise backend to process the logic chain and return the AI-generated response directly in your chat.

**Q: How do I see the past conversational logs for a chatflow via chat?**
Use the 'get_history' tool with the 'chatflow_id'. Your agent will retrieve the past execution traces and logs, helping you understand how users have interacted with that specific logic chain natively.

**Q: Can I list all custom tools configured in my Flowise instance through the agent?**
Absolutely. Use the 'list_tools' tool. Your agent will retrieve custom tools and integrations configured in your environment, allowing you to audit available capabilities through natural conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowise](https://vinkius.com/mcp/flowise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flowise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flowise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flowise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flowise": {
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

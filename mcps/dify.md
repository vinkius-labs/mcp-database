# Dify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage agentic workflows via Dify — send chat messages, track conversations, audit app parameters, and handle file uploads directly from any AI agent.

## Description
Connect your **Dify.ai** application to any AI agent and take full control of your LLM application development and agentic workflows through natural conversation.

### What you can do

- **Agentic Chat Orchestration** — Commands the backend orchestrating absolute explicit strings sending chat messages seamlessly against standard Dify agents
- **Conversation Navigation** — Extracts explicitly attached array vectors representing company-wide conversation listings from your Dify project
- **Message Auditing** — Analyzes specific localized variables decoding active conversation message arrays to track historical interactions
- **Structural Parameters** — Extracts configuration limits mapping global explicit constraints inside the referenced Dify workspace
- **Secure File Ingestion** — Mutate explicit arrays directly transmitting local binaries mapped internally against standard Dify attachments securely
- **Feedback Management** — Submit message-level feedback (likes/dislikes) to instantiate absolute explicit CRM environments tracking AI performance

### How it works

1. Subscribe to this server
2. Enter your Dify API URL and Application-specific API Key (found in your Dify App > API Access)
3. Start managing your agentic workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test and debug Dify agents and RAG pipelines without leaving the development environment
- **Automation Engineers** — manage conversations and upload attachments to Dify apps using natural language
- **Product Teams** — monitor agent performance and verify application parameters in real-time
- **Ops Teams** — audit conversation logs and manage Dify workspace constraints through the chat


## Available Tools (6)
- **chat**: Send a chat message
- **list_conversations**: List conversations
- **list_messages**: List messages in conversation
- **get_parameters**: Get app parameters
- **upload_file**: Upload a file
- **feedback**: Submit message feedback


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a message to my Dify agent: 'Explain the benefits of RAG.'"

**🤖 AI Agent:**
> Dify agent response: 'Retrieval-Augmented Generation (RAG) combines LLMs with external knowledge bases to provide more accurate and context-aware answers...' Would you like to save this to a new conversation?

---

**👤 You:**
> "List my recent Dify conversations for user 'admin_123'"

**🤖 AI Agent:**
> I found 5 recent conversations for 'admin_123'. The latest is 'AI Strategy Discussion' (ID: conv_abc), followed by 'Customer Support Case #456'. Which one would you like to open?

---

**👤 You:**
> "Give a 'like' to message 'msg_789' in Dify"

**🤖 AI Agent:**
> Feedback submitted! I've sent a 'like' for message 'msg_789'. This will help improve the performance tracking of your Dify agent in the dashboard.


## ❓ FAQ

**Q: Can my agent interact with a specific Dify application via chat?**
Yes. When you provide the Application API Key, the agent uses the 'chat' mutation to send your query directly to that Dify agent. It returns the AI response within your current chat context, allowing for seamless integration.

**Q: How do I retrieve the conversation history from my Dify project?**
Use the 'list_conversations' tool. Your agent will pull the explicitly attached array vectors representing your conversation listing. You can then use 'list_messages' with a specific ID to see the detailed interactions.

**Q: Can I upload files to my Dify agents through this server?**
Absolutely. The 'upload_file' tool allows you to transmit local binaries securely. The agent maps these files internally against standard Dify attachments, making them available for your Dify agents to process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dify](https://vinkius.com/mcp/dify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dify": {
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

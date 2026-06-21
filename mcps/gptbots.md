# GPTBots MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gptbots)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage your conversational AI agents, workflows, and knowledge bases via AI.

## Description
Connect your **GPTBots** account to your AI agent and manage your enterprise AI infrastructure conversationally. Interact with your deployed bots, trigger complex automated workflows, and upload new documents to your knowledge bases without leaving your development environment.

### What you can do

- **Bot Interaction** — List active conversations, review chat histories, and send messages directly to your deployed AI agents
- **Knowledge Management** — Browse available knowledge documents and upload new content to keep your bots' context up to date
- **Workflow Automation** — Trigger configured AI workflows and query their execution status programmatically
- **Database Queries** — List tables and records hosted within the GPTBots platform database

### How it works

1. Subscribe to this server
2. Enter your GPTBots API Key and Data Center Region
3. Start managing your AI agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — test bot responses, update knowledge bases, and trigger workflows directly from your IDE
- **Product Managers** — audit conversation histories to evaluate bot performance and user satisfaction
- **Operations Teams** — seamlessly integrate GPTBots automated workflows into your existing daily processes


## Available Tools (8)
- **list_databases**: List tables in the platform database
- **create_knowledge_document**: Upload or create a document in the Knowledge Base
- **get_conversation**: Get details and history of a specific conversation
- **list_conversations**: List chat conversations with a bot
- **list_knowledge_documents**: List documents in a Knowledge Base
- **query_workflow**: Check the execution status of a triggered workflow
- **send_bot_message**: Send a message to a GPTBots Agent
- **trigger_workflow**: Trigger an automated workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GPTBots** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent conversations for bot ID 'bot_123xyz'."

**🤖 AI Agent:**
> Fetching conversations... I found 3 active conversations for this bot. Conversation ID 'conv_987' was updated 5 minutes ago. Would you like to see its chat history?

---

**👤 You:**
> "Trigger the onboarding workflow (ID: 'wf_456') and pass the parameter email='test@example.com'."

**🤖 AI Agent:**
> Triggering workflow... Success! The workflow has been initiated. The execution Record ID is 'rec_789abc'. Let me know if you want me to check its status.


## ❓ FAQ

**Q: How do I chat with a specific bot?**
Use the `send_bot_message` tool and provide the Bot ID and your message content. The AI agent will relay your message to the GPTBots platform and return the bot's response.

**Q: Can I check the status of a triggered workflow?**
Yes. When you use `trigger_workflow`, it returns a Record ID. You can then pass that Record ID to the `query_workflow` tool to monitor its execution status (e.g., Running, Success, Failed).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gptbots](https://vinkius.com/mcp/gptbots)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GPTBots** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gptbots` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GPTBots** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gptbots": {
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

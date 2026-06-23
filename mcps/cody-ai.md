# Cody AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cody-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Enable your AI agent to manage knowledge-base bots, import documents, and query trained AI assistants via the Cody AI API.

## Description
Connect your AI to **Cody AI**, the business AI assistant that can be trained on your own knowledge base.

### What you can do

- **Bot Management** — List active bots, check their configurations, and view which documents they're trained on.
- **Conversations** — Start conversations with any bot and ask questions against your knowledge base.
- **Document Import** — Import web pages and files into specific folders to expand a bot's knowledge.

### How it works

1. Add the Cody AI integration to your AI toolset.
2. Provide your API Key (from Settings > API in the Cody AI dashboard).
3. Manage bots and conversations via natural language.

### Who is this for?

- **Support Teams** — Query trained bots for instant answers to customer questions.
- **Knowledge Managers** — Import new content and manage bot training from chat.
- **Developers** — Integrate Cody AI bots into automated workflows.


## Available Tools (10)
- **create_conversation**: Create a new conversation session with a specific bot
- **get_bot_details**: Retrieve detailed information about a specific bot
- **get_document_status**: Check the syncing status of a document to see if the AI has finished learning it
- **import_webpage**: Import content from a URL into a specific folder in your knowledge base
- **list_bots**: Retrieve all bots configured in your Cody AI account
- **list_conversations**: Retrieve a list of recent conversations
- **list_documents**: Retrieve a list of documents in your knowledge base
- **list_folders**: Retrieve a list of folders in your knowledge base
- **list_messages**: Retrieve the message history for a specific conversation
- **send_message**: Send a prompt to the AI in a specific conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cody AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active bots in Cody AI."

**🤖 AI Agent:**
> You have 3 active bots:
1. 'HR Assistant' — trained on 24 documents, 145 conversations
2. 'Product FAQ' — trained on 12 documents, 89 conversations
3. 'Engineering Wiki' — trained on 56 documents, 210 conversations
Want to start a conversation with any of them?

---

**👤 You:**
> "Ask bot 'bot-xxxx': 'How do I reset my password?'"

**🤖 AI Agent:**
> Bot response (HR Assistant):
"To reset your password, go to Settings > Security > Change Password. If locked out, click 'Forgot Password' on the login page and follow the email instructions."

Sources: employee-handbook.pdf (p.12), security-policy.docx (p.3)

---

**👤 You:**
> "Import my local 'compliance_guidelines.pdf' into the Legal Bot's knowledge base."

**🤖 AI Agent:**
> Upload initiated. 'compliance_guidelines.pdf' has been sent to Cody AI servers. The AI is now training on the new vectors. It will be fully ready to answer policy questions in about 2 minutes.


## ❓ FAQ

**Q: How do I get a Cody AI API key?**
In the Cody AI dashboard, go to **Settings > API** and copy your key. Paste it below.

**Q: What is Focus Mode?**
Focus Mode restricts a bot's knowledge to specific documents for a given conversation, improving answer relevance.

**Q: How long does it take to learn new documents?**
Usually seconds to minutes depending on document size. Use 'get_document_status' to check when sync is complete.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cody-ai](https://vinkius.com/mcp/cody-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cody AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cody-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cody AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cody-ai": {
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

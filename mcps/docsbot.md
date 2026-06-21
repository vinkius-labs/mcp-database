# DocsBot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docsbot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage AI-powered knowledge bases, track sources, and query your bots via the DocsBot API.

## Description
Integrate **DocsBot**, the AI-powered knowledge base platform, directly into your AI workflow. Manage your custom AI bots, track their data sources (URLs, PDFs, documents), monitor indexing status, and query your bots directly using natural language.

### What you can do

- **Bot Oversight** — List and retrieve detailed configuration and metadata for all the AI bots in your team.
- **Knowledge Management** — Monitor data sources used to train your bots and track their last indexing timestamps.
- **Bot Interaction** — Query your bots directly via the agent to retrieve AI-generated answers based on your knowledge base.
- **Analytics & Logs** — Access technical logs of recent bot interactions, including questions and generated answers.

### How it works

1. Connect the DocsBot integration to your AI assistant.
2. Authorize using your DocsBot API Key (found in your account settings).
3. Orchestrate your AI knowledge bases and queries through intuitive conversation.

### Who is this for?

- **Support Teams** — Quickly query documentation bots to assist with customer resolution via chat.
- **Knowledge Managers** — Monitor bot source coverage and indexing status on the go.
- **Product Teams** — Audit bot interaction logs to identify common user questions and content gaps.


## Available Tools (10)
- **ask_bot_question**: Ask a technical question to a specific DocsBot and retrieve an AI-generated answer
- **get_docsbot_account_metadata**: Retrieve metadata for the current authenticated user
- **get_bot_knowledge_summary**: Retrieve a high-level summary of the knowledge base size and source count
- **get_bot_details**: Get detailed settings and information for a specific bot
- **list_recently_indexed_bots**: Identify bots that have had their knowledge base updated recently (mock logic)
- **list_bot_interaction_logs**: List recent questions and answers handled by a specific bot
- **list_team_bots**: List all AI bots configured within a specific team
- **list_bot_knowledge_sources**: List all data sources (URL, PDF, etc.) used to train a specific bot
- **list_docsbot_teams**: List all teams you are a member of in DocsBot
- **search_bot_sources**: Search for specific knowledge sources by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocsBot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask our 'API Docs Bot': 'How do I authenticate using the SDK?'."

**🤖 AI Agent:**
> The bot answered: 'To authenticate using the SDK, you need to initialize the client with your API Key... [detailed steps]'. Should I pull the source links for this answer?

---

**👤 You:**
> "List all data sources used by our 'Support Bot'."

**🤖 AI Agent:**
> I've found 5 sources for the 'Support Bot', including 'help.example.com', 'API-Reference.pdf', and 'Community-FAQs'. 4 sources were successfully indexed today. Would you like to see the last error for the failed source?

---

**👤 You:**
> "Show me the last 5 questions asked to the 'Sales Bot'."

**🤖 AI Agent:**
> The last 5 questions for 'Sales Bot' include: 'What are your pricing plans?', 'Do you offer an annual discount?', and 'How do I upgrade?'. All questions received valid AI answers. Should I pull the detailed logs for any of them?


## ❓ FAQ

**Q: How do I get a DocsBot API Key?**
Log in to your DocsBot account, navigate to the API section in your account settings, and you can generate or retrieve your unique API Key from there.

**Q: Can the agent train my bots?**
This integration currently focuses on querying bots and auditing sources. Adding new sources or triggering full training cycles should be managed via the DocsBot dashboard.

**Q: Which AI models are used?**
DocsBot supports various models including GPT-3.5 and GPT-4. The agent will retrieve results based on the specific model configured for your bot in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docsbot](https://vinkius.com/mcp/docsbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DocsBot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docsbot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DocsBot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docsbot": {
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

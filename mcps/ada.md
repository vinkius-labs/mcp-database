# Ada MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ada)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

AI-powered customer service automation — manage conversations, end users, and knowledge via AI.

## Description
Connect your **Ada** account to your AI agent to unlock advanced customer service automation. From monitoring real-time conversations to managing your knowledge base and syncing user metadata, your agent handles conversational AI orchestration through natural language.

### What you can do

- **Conversation Oversight** — List and retrieve details of active or past support conversations to identify trends
- **End User Management** — Manage user profiles and sync metadata (metavariables) between Ada and your external systems
- **Knowledge Management** — Create, update, and list articles in your knowledge base to help your AI agent provide better answers
- **Real-time Analytics** — Retrieve insights on automated resolution rates and agent handoff patterns
- **Compliance Support** — Manage data privacy requests and conversation retention directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Ada Platform Token and Handle
3. Start managing your AI support ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Experience Managers** — monitor automated conversation quality and identify automation gaps
- **Support Operations Teams** — sync user data and manage knowledge base articles efficiently
- **Developers** — integrate Ada's conversational AI into custom applications and workflows
- **AI Training Leads** — audit bot responses and update knowledge sources instantly


## Available Tools
- **list_conversations**: Retrieve active and past customer support conversations handled by the Ada bot
- **get_end_user**: Requires the End User ID.

Retrieve profile information and custom metavariables for a specific Ada end user
- **list_articles**: Retrieve the catalog of help articles used by the Ada AI agent to answer customer queries
- **create_article**: Needs title and text content.

Add a new text article to the Ada knowledge base to immediately improve AI bot responses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ada** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 conversations handled by Ada."

**🤖 AI Agent:**
> I've retrieved the last 5 conversations. 4 were resolved automatically and 1 was handed off to a human agent. Would you like to see the transcript for any of them?


## ❓ FAQ

**Q: Can I update my knowledge base via the agent?**
Yes! Use the `create_article` tool to add new information to your Ada knowledge base. This helps the AI bot stay up-to-date with your latest product or policy changes.

**Q: What are the API rate limits on Ada?**
The default platform API limit is 10,000 requests per day (10 per second). Some specific endpoints, such as the Data Export API, have additional limits like 15,000 requests per day.

**Q: Are there quotas per knowledge article in Ada?**
Yes, Knowledge Base APIs enforce a constraint of 100KB per individual article, up to a maximum limit of 50,000 global articles in your organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ada](https://vinkius.com/mcp/ada)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ada** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ada` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ada** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ada": {
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

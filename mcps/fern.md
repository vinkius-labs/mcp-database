# Fern MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fern)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and interact with Fern documentation platforms — generate access tokens, index websites for AI, and query analytics directly from your agent.

## Description
Connect to the **Fern** ecosystem to supercharge your documentation workflows. This server allows AI agents to manage documentation access, trigger AI indexing, and interact with the 'Ask Fern' assistant.

### What you can do

- **AI Chat Completion** — Interact with the Ask Fern AI assistant to get answers from specific documentation domains using `post_chat_completion`.
- **Website Indexing** — Trigger new crawling and indexing jobs via `index_website` to keep your documentation searchable and AI-ready.
- **Access Management** — Generate JWTs and Algolia search keys for secure documentation access using `get_jwt` and `get_search_key`.
- **Analytics & Insights** — Retrieve recent user queries and analytics with `get_recent_queries` to understand how people interact with your docs.
- **User Verification** — Quickly check authentication status and user details with the `whoami` tool.

### How it works

1. Subscribe to this server
2. Enter your Fern API Key and Token
3. Start managing your documentation lifecycle from your favorite AI client

### Who is this for?

- **Documentation Engineers** — automate the indexing of new content and monitor search analytics.
- **Support Teams** — use the Ask Fern AI to find answers across complex documentation domains.
- **Developers** — programmatically manage access keys and verify user permissions.


## Available Tools (6)
- **post_chat_completion**: Interact with the Ask Fern AI assistant
- **whoami**: Get current user information
- **get_jwt**: Get JWT from Fern API key
- **get_recent_queries**: Get recent queries and analytics
- **get_search_key**: Get Algolia search credentials
- **index_website**: Start crawling and indexing a website for Ask Fern


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fern** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Ask Fern: 'What is the rate limit?' for the domain 'docs.example.com'"

**🤖 AI Agent:**
> I've sent your question to Ask Fern for the 'docs.example.com' domain. The assistant responds: 'The current rate limit is 100 requests per minute for the free tier and 5000 for enterprise users.'

---

**👤 You:**
> "Start indexing the website https://docs.example.com for the 'main' domain."

**🤖 AI Agent:**
> I've triggered a new indexing job for 'https://docs.example.com' under the 'main' domain. You can check the status in your Fern dashboard.

---

**👤 You:**
> "Show me the recent queries for the 'api-docs' domain."

**🤖 AI Agent:**
> Retrieving analytics for 'api-docs'... Recent questions include: 'How to use webhooks?', 'Authentication error 401', and 'SDK installation guide'.


## ❓ FAQ

**Q: Can I use the AI assistant to query my documentation?**
Yes, use the `post_chat_completion` tool with your documentation domain and a list of messages. The agent will interact with the Ask Fern assistant to provide relevant answers.

**Q: How do I update the search index for a new site?**
Use the `index_website` tool by providing the documentation domain and the base URL you want to crawl. This will trigger a new indexing job for the Ask Fern assistant.

**Q: How can I see what my users are searching for?**
The `get_recent_queries` tool allows you to retrieve analytics and recent questions asked by users on a specific documentation domain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fern](https://vinkius.com/mcp/fern)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fern** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fern` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fern** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fern": {
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

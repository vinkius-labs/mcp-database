# Omnivore (Read-Later) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omnivore-read-later)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Omnivore library — search articles, read full content, and save new links directly from your AI agent.

## Description
Connect your **Omnivore** account to any AI agent to organize your reading list and extract knowledge from saved articles using natural language.

### What you can do

- **Search & Filter** — Use the `search_articles` tool to find content using labels, folders, or read status (e.g., 'is:unread label:AI')
- **Full Content Retrieval** — Use `get_article` to fetch the complete text, author, and labels for deep analysis or summarization
- **Quick Saving** — Use `save_url` to instantly add new web links to your library without leaving your conversation
- **User Profile** — Use `get_me` to verify your account details and connection status

### How it works

1. Subscribe to this server
2. Enter your Omnivore API Key
3. Start managing your reading list from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — quickly find and analyze saved papers or articles within their library
- **Content Creators** — retrieve source material and inspiration from their curated reading list
- **Knowledge Workers** — maintain a seamless flow between reading and acting on information


## Available Tools
- **get_article**: Get full content of a specific article
- **get_me**: Get current Omnivore user details
- **save_url**: Save a URL to Omnivore library
- **search_articles**: g., label:Newsletter, in:inbox, is:unread, has:highlights) to find articles.

Search and filter articles in Omnivore library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omnivore (Read-Later)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Omnivore library for unread articles about 'Machine Learning'."

**🤖 AI Agent:**
> I found 3 unread articles about Machine Learning. The most recent is 'Understanding Transformers' (slug: understanding-transformers). Would you like me to fetch the full content of any of these?

---

**👤 You:**
> "Fetch the full content of the article with slug 'mcp-guide' for username 'alex_dev'."

**🤖 AI Agent:**
> I've retrieved the article 'The Ultimate MCP Guide'. It covers the Model Context Protocol architecture and implementation details. Would you like a summary of the key points?

---

**👤 You:**
> "Save the URL 'https://blog.omnivore.app/p/getting-started' to my library."

**🤖 AI Agent:**
> Successfully saved the URL to your Omnivore library. It is now available in your inbox for later reading.


## ❓ FAQ

**Q: Can I filter my search by labels or read status?**
Yes. Use the `search_articles` tool with Omnivore's search syntax, such as `label:AI` or `is:unread`, to narrow down your results.

**Q: How do I get the actual text of a saved page for analysis?**
Use the `get_article` tool by providing the article's unique slug and the owner's username. The agent will retrieve the full text content and metadata.

**Q: Is it possible to add new links to my library via the agent?**
Yes, the `save_url` action allows you to send any web link directly to your Omnivore library for later reading.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omnivore-read-later](https://vinkius.com/mcp/omnivore-read-later)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Omnivore (Read-Later)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `omnivore-read-later` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Omnivore (Read-Later)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omnivore-read-later": {
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

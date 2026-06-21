# Readwise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/readwise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Equip your AI to directly search, read, and retrieve your unified digital highlights, books, and Reader documents stored in Readwise.

## Description
Connect your **Readwise** account directly to your AI agent. Enabling this integration turns your AI into an expert research assistant, capable of instantly scanning your entire timeline of book highlights, article snippets, tweet saves, and personal tags directly from your unified Readwise and Readwise Reader library.

### What you can do

- **Highlight Retrieval** — Perform searches or bulk retrievals of every snippet, quote, or highlight you've ever saved from your Kindle, Apple Books, and web browsers.
- **Library Browsing** — Ask your AI to list all the books, articles, and sources currently populated in your Readwise database.
- **Readwise Reader Documents** — Full access to list and extract content directly from articles and feeds saved into your Readwise Reader app.
- **Tag Management Analysis** — Retrieve the categorizations and tags you use to organize your knowledge base system.

### How it works

1. Authorize the Readwise MCP server in your workspace.
2. Provide your Readwise Access Token (generated directly from `readwise.io/access_token`).
3. Chat with your AI to immediately start synthesizing ideas, drafting essays, or finding specific quotes from your personal reading history.

### Who is this for?

- **Researchers & Writers** — Recall specific quotes from past books and synthesize notes into comprehensive research drafts without breaking focus.
- **Students & Academics** — Easily query your centralized highlights from PDFs or class reading materials to build study guides.
- **Knowledge Workers** — Transform casual web highlighting into an active second brain, allowing AI to connect ideas across different saved articles.


## Available Tools
- **check_auth_status**: Verifies the validity of the Readwise access token
- **get_reader_document**: Retrieves details for a specific Reader document
- **list_books**: Lists all books and sources in Readwise
- **list_highlights**: Lists all highlights from the user's Readwise account
- **list_reader_documents**: Lists documents in the Readwise Reader
- **list_tags**: Lists all tags used in Readwise


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Readwise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent 5 books I highlighted on Readwise."

**🤖 AI Agent:**
> Using the `list_books` endpoint, I found your latest highlighted sources. The top results are: 'Atomic Habits' (ID: 9234), 'Deep Work' (ID: 8812), and 'Sapiens' (ID: 8129).

---

**👤 You:**
> "Show me the text of the recent document I saved to Reader with the ID 1234."

**🤖 AI Agent:**
> Executing `get_reader_document` for ID 1234. I've fetched the full Markdown of the article. It’s titled 'The Future of AI Tools', summarizing context on how autonomous agents reshape programming workflows from start to finish.

---

**👤 You:**
> "Search my highlights for any mentions of 'productivity'."

**🤖 AI Agent:**
> I queried `list_highlights` and filtered your collection. You have 15 highlights mentioning 'productivity'. One standout quote from 'Deep Work' says: 'To produce at your peak level you need to work for extended periods with full concentration.'


## ❓ FAQ

**Q: Where do I obtain my Readwise Access Token?**
You can quickly find or generate your specific access token by logging into your Readwise account and directly visiting `https://readwise.io/access_token`. Copy the alphanumeric token presented there and insert it directly into the prompt required by this integration.

**Q: Can the AI add native highlights or upload PDFs to Reader for me?**
Currently, the integration server functions on a Read-Only standard format designed specifically to fetch existing knowledge. It fetches metadata or full-text values from highlights, tags, and Reader items, but it doesn't support publishing or updating new sources back to Readwise natively.

**Q: Does it also search through to my saved Readwise Reader feed?**
Yes. Tools like `list_reader_documents` and `get_reader_document` are designated explicitly for extracting articles or stored reads directly residing inside your connected Readwise Reader account, keeping both typical highlights and Reader data separate but reachable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readwise](https://vinkius.com/mcp/readwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Readwise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `readwise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Readwise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "readwise": {
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

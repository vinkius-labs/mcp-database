# Exa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exa-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Find exactly the web content you need with semantic search that understands context and returns high-quality curated results.

## Description
Connect **Exa (formerly Metaphor)** to any AI agent and simplify how you discover relevant web data, research topics using neural embeddings, and extract cleaned content through natural conversation.

### What you can do

- **Neural Search** — Perform AI-powered searches that understand the meaning and intent of your query, not just keywords.
- **Semantic Similarity** — Find web pages and articles that are semantically similar to a specific seed URL.
- **Content Extraction** — Fetch cleaned, readable text and metadata from multiple URLs or page IDs in a single request.
- **Research Automation** — Discover high-quality sources and analyze web content programmatically via AI.
- **Data Insights** — retrieve comprehensive metadata for search results to identify top-performing resources.
- **Intelligent Discovery** — Use 'Autoprompt' to automatically optimize your queries for neural search accuracy.

### How it works

1. Subscribe to this server
2. Enter your Exa API Key (found in your account dashboard)
3. Start searching the web for your AI projects from Claude, Cursor, or any MCP client

### Who is this for?

- **AI Developers & Researchers** — quickly find semantically relevant data and clean web content via simple AI commands.
- **Content Strategists** — discover similar articles and research topics across the web directly from the workspace.
- **Knowledge Workers** — automate information discovery and extract key insights via the AI assistant.


## Available Tools
- **answer**: Get an AI answer
- **find_similar**: Great for competitive analysis and research.

Find similar pages
- **find_similar_with_contents**: Find similar pages with content
- **get_contents**: Extract page contents
- **search_domain**: Useful for site-specific research or documentation lookups.

Search within a domain
- **search_keyword**: Traditional keyword search
- **search_neural**: Ideal for conceptual queries and research topics.

Neural semantic search
- **search_recent**: Ideal for news and trending topics.

Search recent content
- **search**: Returns titles, URLs, and relevance scores for matching pages.

Search the web with AI
- **search_with_contents**: Search and extract page content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Neural search for 'the latest breakthroughs in room-temperature superconductors'."

**🤖 AI Agent:**
> I've performed a neural search for you. I found 10 high-quality links including recent pre-prints from arXiv, specialized science blogs, and official university press releases. Which source would you like me to extract the content from?

---

**👤 You:**
> "Find 5 links similar to 'https://openai.com/blog/instruction-following'."

**🤖 AI Agent:**
> Fetching similar content... I've identified 5 semantically related articles, including papers on RLHF from Anthropic, Google DeepMind's blog on fine-tuning, and technical breakdowns from HuggingFace. Shall I retrieve the metadata for these?

---

**👤 You:**
> "Extract the cleaned text content from 'https://arxiv.org/abs/2312.00752'."

**🤖 AI Agent:**
> Extraction complete! I've retrieved the cleaned text content for the arXiv paper (ID: 2312.00752). It contains the abstract, full body text, and author metadata. Would you like me to summarize the key findings for you?


## ❓ FAQ

**Q: Can I perform a meaning-based search instead of keywords via AI?**
Yes! Use the `search` tool. Provide your query and enable `useAutoprompt`. Exa will use its neural embeddings to find links that match the intent of your question.

**Q: How do I find articles similar to a specific URL?**
Use the `find_similar` tool. Provide the seed URL, and the agent will retrieve a list of pages that are semantically related to that content.

**Q: Is it possible to extract cleaned text from multiple pages via AI?**
Absolutely. Use the `get_contents` query. Provide an array of URLs or Exa IDs, and the agent will return the cleaned text content and metadata for each page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exa-alternative](https://vinkius.com/mcp/exa-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `exa-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exa-alternative": {
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

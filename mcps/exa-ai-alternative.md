# Exa AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exa-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Search the web with neural embeddings that understand meaning, not just keywords, and return the most relevant results for any query.

## Description
Connect your **Exa AI** (formerly Metaphor) account to any AI agent and take full control of your web research and data extraction workflows through natural conversation.

### What you can do

- **Semantic Search Orchestration** — Perform AI-native searches that understand intent and meaning to retrieve the most relevant web pages programmatically
- **Content Intelligence** — Programmatically extract clean, parsed text or highlights from any URL, excluding ads and boilerplate automatically
- **Similarity Discovery** — Find pages semantically similar to a source URL to build comprehensive and high-fidelity research datasets
- **Deep Data Mapping** — Discover all reachable links on a domain and retrieve discovery metadata to understand site structures programmatically
- **Search Filtering** — Restricted searches by domain, category (company, blog, news), or discovery date directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Exa AI dashboard (Settings > API Keys)
3. Start searching the web semantically from Claude, Cursor, or any MCP client

No more manual keyword-based searching or messy scraping scripts. Your AI acts as your dedicated neural research assistant.

### Who is this for?

- **AI Developers** — build RAG pipelines by programmatically ingesting semantically relevant web data using natural language
- **Market Researchers** — instantly identify competitors and find similar companies across the web using semantic discovery
- **Content Analysts** — automate the extraction of highlights and clean text from technical blogs and news without leaving your workspace


## Available Tools (12)
- **keyword_search**: Search by exact keywords
- **advanced_custom_search**: Complex search query
- **find_similar_pages**: Find matches for a URL
- **get_api_status**: Check connection
- **extract_page_content**: Retrieve web page text
- **get_query_highlights**: Extract relevant snippets
- **perform_live_crawl**: Fresh web extraction
- **search_with_contents**: Search and extract text
- **search_by_category**: Search by site type
- **search_by_crawl_date**: Search by discovery date
- **search_specific_domains**: Search within sites
- **semantic_search**: Perform AI-native search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exa AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest research on room-temperature superconductors using Exa."

**🤖 AI Agent:**
> Running semantic search... I've found 5 high-quality research papers and articles from the last 3 months. Notable results include a study from Nature and a detailed technical blog from MIT. Would you like the highlights for any of these?

---

**👤 You:**
> "Find pages similar to 'https://openai.com/blog/sora/' from news domains."

**🤖 AI Agent:**
> Discovery complete! I've located 3 semantically similar articles on news platforms like TechCrunch and The Verge. They discuss generative video trends and competitor reactions. Shall I extract the clean text from these links?

---

**👤 You:**
> "Get the clean text content from 'https://en.wikipedia.org/wiki/Artificial_intelligence'."

**🤖 AI Agent:**
> Extraction complete! I've retrieved the clean Markdown content for the AI Wikipedia page. It includes the history, definitions, and main research areas, excluding all sidebars and ads. Would you like a summary?


## ❓ FAQ

**Q: How do I find my Exa AI API Key?**
Log in to your [**Exa AI dashboard**](https://dashboard.exa.ai/), and copy your unique API Key from the settings section.

**Q: What makes semantic search different?**
Traditional search uses keywords. Semantic search uses neural embeddings to understand the meaning and context of your query, finding better matches.

**Q: Can I extract text from multiple URLs at once?**
Yes! The `extract_page_content` tool accepts a JSON array of URLs and retrieves the parsed content for all of them programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exa-ai-alternative](https://vinkius.com/mcp/exa-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exa AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exa-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exa AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exa-ai-alternative": {
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

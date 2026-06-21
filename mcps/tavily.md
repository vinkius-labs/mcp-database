# Tavily MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tavily)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search the web for AI — audit search context, answers, and extracted content via AI.

## Description
Empower your AI agent to orchestrate your entire web research workflow with **Tavily**, the search engine built specifically for AI agents. By connecting Tavily to your agent, you transform complex information retrieval into a natural conversation. Your agent can instantly audit search context, retrieve direct AI answers, and extract clean content from any URL without you ever touching a browser. Whether you are conducting deep market research or monitoring real-time news, your agent acts as a real-time research assistant, ensuring your intelligence is always grounded in optimized, high-quality data.

### What you can do

- **AI-Optimized Search** — Query the web for results specifically curated for LLM consumption, including snippets and relevancy scores.
- **Direct Answers** — Retrieve concise AI-generated answers for complex search queries to skip manual data synthesis.
- **Content Extraction** — Extract clean, readable text from any list of URLs to maintain a structured view of web content.
- **Real-time News Oversight** — Monitor current events through specialized news search to stay on top of industry updates.
- **Visual Discovery** — Search for high-quality images optimized for AI agents to maintain visual context in your research.

### How it works

1. Subscribe to this server
2. Enter your Tavily API Key
3. Start managing your web research through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Developers** — monitor search contexts and optimize agent information retrieval straight from your workflow.
- **Researchers & Analysts** — verify information sources and extract content from multiple sites without manual browsing.
- **Content Strategists** — perform rapid audits of trending topics and retrieve AI answers for content planning.
- **Operations Leads** — automate research querying to orchestrate cross-functional intelligence teams smoothly.


## Available Tools (6)
- **extract_content**: Extract clean content from specific URLs
- **get_answer**: Get a direct AI answer for a search query
- **get_search_context**: Get search context for a query (optimized for LLMs)
- **search_images**: Search for images optimized for AI
- **search_news**: Search for real-time news results
- **search_web**: Search the web for AI-optimized results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tavily** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest breakthroughs in 'Quantum Computing' using Tavily."

**🤖 AI Agent:**
> I've retrieved the latest research context. Recent breakthroughs include new error-correction methods and increased qubit coherence times. Would you like the links to the full papers?

---

**👤 You:**
> "Get an AI answer for 'How does photosynthesis work?'."

**🤖 AI Agent:**
> According to the latest sources, photosynthesis is the process used by plants to convert light energy into chemical energy. I can provide a more detailed breakdown if needed.

---

**👤 You:**
> "Extract content from https://vinkius.com."

**🤖 AI Agent:**
> Content extracted! I've retrieved the main text from Vinkius, which discusses their latest AI research and MCP server ecosystem. Would you like a summary of the findings?


## ❓ FAQ

**Q: How do I find my Tavily API Key?**
Log in to your [**Tavily dashboard**](https://tavily.com/), and you will find your API Key on the overview page. Copy and paste it below.

**Q: What is Search Context vs Web Search?**
Search Context is optimized for direct ingestion by LLMs, providing a denser format of information, while Web Search provides standard curated results with snippets and scores.

**Q: Can the agent extract content from any website?**
Yes. The `extract_content` tool allows your agent to retrieve the cleaned main text from any accessible URL, bypassing ads and navigation elements for structured analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tavily](https://vinkius.com/mcp/tavily)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tavily** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tavily` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tavily** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tavily": {
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

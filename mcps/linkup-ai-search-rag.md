# Linkup (AI Search & RAG) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkup-ai-search-rag)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Power your AI agents with real-time web search via Linkup — execute semantic queries and extract RAG-ready content.

## Description
Connect your **Linkup** account to any AI agent and take full control of real-time web intelligence and content retrieval for RAG pipelines through natural conversation.

### What you can do

- **Semantic Web Search** — Execute context-rich queries that return high-relevancy results specifically optimized for Large Language Models directly from your agent
- **Deep Content Retrieval** — Extract clean, readable text from any web URL, stripping away noise and navigation to feed high-quality grounding data to your AI
- **RAG-Ready Payloads** — Retrieve structured search results including titles, snippets, and source URLs designed for seamless integration into vector stores
- **Precision Extraction** — Target specific URLs for content parsing, ensuring your agent has the exact technical context or documentation required for its task
- **Real-time Intelligence** — Access the latest facts and data from across the internet to ground your agent's answers in up-to-date reality
- **Search Breadth** — Switch between standard and deep search modes to balance between rapid fact-finding and comprehensive research across the web

### How it works

1. Subscribe to this server
2. Enter your Linkup API Key
3. Start grounding your AI with live web data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **RAG Developers** — provide your agents with real-time web access and precise document retrieval for contextual grounding through natural conversation
- **AI & ML Engineers** — automate the extraction of high-quality web content for model fine-tuning and evaluation datasets
- **Market Researchers** — perform large-scale data collection and fact-finding across the web without manual scraping scripts


## Available Tools
- **search_web**: Choose "fast" mapping for basic factual requests and "deep" for thorough research limits.

Perform a real-time web search extracting deep answers utilizing Linkup Platform
- **fetch_url**: Bypasses advanced bot protections executing complex SPA JavaScript loops automatically.

Fetch and extract clean content from any specific URL using Linkup Platform


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linkup (AI Search & RAG)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest NVIDIA earnings report summary"

**🤖 AI Agent:**
> Searching the web… Based on the latest results from Linkup, NVIDIA reported Q4 revenue of $22.1 billion, up 265% year-over-year. Data center revenue hit a record $18.4 billion. Would you like me to fetch the full detailed analysis from one of the source articles?

---

**👤 You:**
> "Extract the technical specifications from this documentation URL: [url]"

**🤖 AI Agent:**
> Fetching content… I've extracted the clean technical text. The system requirements include 16GB RAM, an NVIDIA RTX 30-series GPU, and Python 3.10+. I can provide the full list of API endpoints described in the doc as well.

---

**👤 You:**
> "Deep search for 'AI agent security best practices 2024'"

**🤖 AI Agent:**
> Performing deep search… I've synthesized security insights from 12 diverse sources. Key best practices for 2024 include: 1) Strict tool-call sandboxing, 2) Human-in-the-loop for high-stakes actions, 3) Real-time prompt injection monitoring. Would you like a detailed breakdown of the sandboxing techniques?


## ❓ FAQ

**Q: How can Linkup help my agent provide more up-to-date answers?**
Use the `linkup_search` tool to give your agent access to live web data. By performing semantic searches across the internet, your agent can retrieve the latest news, reports, and documentation, grounding its answers in current facts.

**Q: Can I extract clean text from a specific URL for RAG?**
Yes. The `linkup_fetch` tool is specifically designed for content extraction. It renders the target page and returns a clean text version stripped of navigation and ads, making it ideal for feeding high-quality context to your agent.

**Q: What is the difference between standard and deep search modes?**
Standard search focuses on rapid fact-finding and top results. Deep search performs a more comprehensive crawl across many more sources, which is better for complex research tasks that require diverse perspectives and detailed data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkup-ai-search-rag](https://vinkius.com/mcp/linkup-ai-search-rag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linkup (AI Search & RAG)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `linkup-ai-search-rag` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linkup (AI Search & RAG)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkup-ai-search-rag": {
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

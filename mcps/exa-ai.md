# Exa AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exa-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search and discover the web — audit semantic results and similar links via AI.

## Description
Empower your AI agent to orchestrate your entire web discovery and semantic search workflow with **Exa AI**, the search engine built for the future of AI. By connecting Exa to your agent, you transform complex information gathering into a natural conversation. Your agent can instantly search the web using semantic embeddings, audit similar websites through URL matching, and retrieve cleaned page content without you ever touching a browser. Whether you are conducting deep market research or monitoring niche industry trends, your agent acts as a real-time web analyst, ensuring your intelligence is always grounded in contextually relevant data.

### What you can do

- **Semantic Auditing** — Query the web using natural language and retrieve results based on meaning rather than just keywords.
- **Similar Discovery** — Find websites similar to any provided URL to identify competitors or related sources instantly.
- **Content Oversight** — Retrieve cleaned HTML or text content for any search result to maintain a structured view of web data.
- **Usage Intelligence** — Monitor your API usage and crawl statistics to maintain strict control over your research budget.
- **Unified Search** — Perform search and content retrieval in a single request to optimize agent response times.

### How it works

1. Subscribe to this server
2. Enter your Exa API Key
3. Start managing your web discovery through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Research Analysts** — monitor semantic search results and competitor links straight from your workflow.
- **AI Developers** — verify content extraction and audit search relevancy for your agentic applications.
- **Knowledge Workers** — perform rapid audits of related sources and retrieve site summaries through natural language.
- **Operations Leads** — automate web discovery querying to orchestrate cross-functional research teams smoothly.


## Available Tools (4)
- **find_similar**: Note: this endpoint is deprecated by Exa and may be removed in the future.

Find websites similar to a given URL (deprecated — use search instead)
- **get_contents**: Retrieve cleaned text content for specific page IDs
- **search_with_contents**: Search the web and retrieve page contents in one request
- **search_web**: Returns URLs, titles, and metadata.

Search the web semantically using Exa AI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exa AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find 5 high-quality research papers about 'Climate Change mitigation' using Exa."

**🤖 AI Agent:**
> I've retrieved 5 highly relevant research papers. Notable results include studies on carbon capture and renewable energy adoption. Would you like the links and summaries for each?

---

**👤 You:**
> "Find sites similar to https://techcrunch.com."

**🤖 AI Agent:**
> I've found 10 sites similar to TechCrunch. Top matches include VentureBeat, The Verge, and Wired. I can provide the relevancy scores for each if you'd like.

---

**👤 You:**
> "Search for 'future of AI robotics' and give me the full content of the best result."

**🤖 AI Agent:**
> Search complete! The top result is a detailed analysis from MIT. I've retrieved the cleaned content, which discusses embodied AI and humanoid developments. Would you like a summary?


## ❓ FAQ

**Q: How do I find my Exa API Key?**
Log in to your [**Exa.ai dashboard**](https://dashboard.exa.ai/), and you will find your API Key on the API Keys page. Copy and paste it below.

**Q: What makes Exa search 'semantic'?**
Exa uses neural embeddings to understand the meaning behind your query, allowing it to find results that are contextually related even if they don't share exact keywords.

**Q: Can the agent find sites similar to a blog post?**
Yes. Use the `find_similar` tool providing the URL of the blog post. Your agent will return a list of sources with similar topics or writing styles instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exa-ai](https://vinkius.com/mcp/exa-ai)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `exa-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exa AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exa-ai": {
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

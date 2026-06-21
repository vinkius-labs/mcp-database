# Olostep MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/olostep)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scrape web pages at scale with a headless browser API that renders JavaScript and returns clean structured data instantly.

## Description
Connect your **Olostep** account to any AI agent and take full control of your web scraping orchestration and automated data extraction workflows through natural conversation.

### What you can do

- **Scraping Batch Orchestration** â€” List and manage your entire portfolio of scraping batches programmatically, retrieving detailed technical status and URL counts
- **URL Extraction Intelligence** â€” Programmatically trigger and monitor real-time URL scrapes to maintain a perfectly coordinated knowledge pipeline
- **Agent & Schedule Architecture** â€” Access your complete directory of research agents and automated schedules to oversee your organizational data ingestion
- **Hosted Result Monitoring** â€” Access hosted result URLs (Markdown, JSON) and retrieve technical metadata for your research archive in real-time
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor scraping volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Olostep dashboard (Settings > API)
3. Start orchestrating your data growth from Claude, Cursor, or any MCP client

No more manual checking of individual scraping jobs or missing batch completion alerts. Your AI acts as your dedicated data coordinator and extraction architect.

### Who is this for?

- **Data Engineers** â€” instantly retrieve batch performance recaps and monitor scraping status using natural language commands
- **Researchers** â€” verify individual URL metadata and track extraction history without leaving your creative workspace
- **Developers** â€” integrate high-speed Olostep scraping data into custom LLM and RAG pipelines through simple AI queries


## Available Tools
- **check_olostep_status**: Verify Olostep API connectivity
- **create_agent**: Create a scraping agent
- **create_batch**: Pass URLs as comma-separated values.

Create a batch scrape
- **get_agent**: Get agent details
- **get_batch_results**: Get batch results
- **get_batch**: Get batch details
- **get_usage**: Get API usage stats
- **list_agents**: List scraping agents
- **list_batches**: List all batches
- **scrape_url**: Optionally specify format: markdown, html, or text.

Scrape a web page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Olostep** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the homepage of example.com as markdown."

**🤖 AI Agent:**
> Page scraped successfully. The content is 2,400 words with 15 images and 8 links. Here's the markdown output. Would you like to save it or scrape additional pages?

---

**👤 You:**
> "Create a batch scrape for 5 competitor product pages."

**🤖 AI Agent:**
> Batch created with 5 URLs. Job ID: BATCH-7291. Processing has started — 2 of 5 pages already completed. Would you like me to check back when all are done?

---

**👤 You:**
> "Show my Olostep API usage this month."

**🤖 AI Agent:**
> This month: 1,245 pages scraped, 82 batch jobs, 340 MB bandwidth used. You have 8,755 credits remaining on your plan. Would you like to see agent-level breakdown?


## ❓ FAQ

**Q: How do I scrape a web page via AI?**
Use the `scrape_url` tool with the target URL and optional format (markdown, html, or text). The content is extracted and returned instantly.

**Q: Can I scrape multiple URLs at once?**
Yes. Use `create_batch` with comma-separated URLs to submit a batch job. Track progress with `get_batch` and retrieve results with `get_batch_results`.

**Q: What are scraping agents and how do I use them?**
Agents are reusable scraping configurations with custom extraction rules. Use `create_agent` to set one up and `list_agents` to manage them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/olostep](https://vinkius.com/mcp/olostep)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Olostep** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `olostep` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Olostep** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "olostep": {
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

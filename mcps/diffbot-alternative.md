# Diffbot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diffbot-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Extract structured data from any web page using AI that understands content like a human and builds knowledge graphs automatically.

## Description
Connect your **Diffbot** account to any AI agent and take full control of your structured data extraction and knowledge graph research workflows through natural conversation.

### What you can do

- **Web Content Orchestration** — Extract structured metadata from any URL programmatically using AI models specialized for articles, products, and discussion threads
- **Knowledge Graph Intelligence** — Query Diffbot's massive database of billions of entities using DQL to find organization firmographics, people profiles, and market signals
- **Entity Enrichment** — Programmatically enhance person and company profiles using names or domains to maintain a high-fidelity database of leads and competitors
- **Analyze & Identify** — Automatically detect the page type of any URL to apply the most accurate extraction model directly through your agent
- **Crawl Monitoring** — List and monitor active crawling jobs and check your account usage and API status for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your Diffbot dashboard
3. Start extracting structured web data from Claude, Cursor, or any MCP client

No more manual copy-pasting or complex web scraping scripts. Your AI acts as your dedicated data engineer and market research analyst.

### Who is this for?

- **Data Engineers** — instantly extract structured data from thousands of URLs using natural language commands
- **Market Researchers** — search the Knowledge Graph for specific industry signals and company data without leaving your workspace
- **Growth Marketers** — automate lead enrichment and competitive analysis through simple AI queries


## Available Tools (11)
- **analyze_page_type**: Auto-detect page type
- **enhance_company_profile**: Enrich company data
- **enhance_person_profile**: Enrich person data
- **extract_article_data**: Extract news/blog post
- **extract_forum_thread**: Extract forum/comments
- **extract_images**: Identify primary images
- **extract_product_data**: Extract e-commerce info
- **extract_video_metadata**: Identify embedded videos
- **search_knowledge_graph**: g. type:Organization industries:"AI").

Query world entities
- **verify_api_credentials**: Verify your Diffbot API credentials
- **list_active_crawls**: Check crawl status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diffbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the main content from the article at 'https://vinkius.com/blog/mcp-standards'."

**🤖 AI Agent:**
> Article extraction triggered! I've retrieved the clean text, author 'John Doe', and a positive sentiment score. Would you like me to extract any discussion threads from the page as well?

---

**👤 You:**
> "Search for companies in 'San Francisco' with more than 1000 employees using DQL."

**🤖 AI Agent:**
> Querying Knowledge Graph... I found 15 organizations matching your criteria. Highlights include 'Salesforce' and 'Uber'. Would you like the detailed firmographics for these entities?

---

**👤 You:**
> "Enhance the company profile for 'Vinkius' using domain 'vinkius.com'."

**🤖 AI Agent:**
> Profile enhanced! Vinkius is identified as a 'Technology' organization based in Portugal. I've retrieved their social links, employee count, and latest funding metadata. Shall I search for their key people?


## ❓ FAQ

**Q: How do I find my Diffbot API Token?**
Log in to your Diffbot account and navigate to the **Dashboard** or **Manage Tokens** section to copy your unique access token.

**Q: What is DQL and how can I use it?**
DQL (Diffbot Query Language) allows you to filter the Knowledge Graph. Use the `search_knowledge_graph` tool with queries like `type:Organization industries:"AI"`.

**Q: Can I extract comments from articles?**
Yes! The `extract_article_data` tool has an optional `discussion` parameter. Set it to `true` to retrieve structured comment threads if available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diffbot-alternative](https://vinkius.com/mcp/diffbot-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diffbot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diffbot-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diffbot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diffbot-alternative": {
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

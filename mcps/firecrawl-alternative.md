# Firecrawl MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firecrawl-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Scrape and crawl the web — audit website content and maps via AI.

## Description
Empower your AI agent to orchestrate your entire web extraction workflow with **Firecrawl**, the engine that turns websites into LLM-ready markdown. By connecting Firecrawl to your agent, you transform complex scraping tasks into a natural conversation. Your agent can instantly scrape specific URLs, audit website structure through mapping, and manage long-running crawl jobs without you ever touching a technical dashboard. Whether you are building a knowledge base or monitoring competitor updates, your agent acts as a real-time web curator, ensuring your data is always structured and up-to-date.

### What you can do

- **Web Auditing** — Scrape any URL and retrieve cleaned markdown content to maintain a structured view of site information.
- **Crawl Oversight** — Start multi-page crawl jobs and monitor their progress to ensure comprehensive data collection.
- **Structural Intelligence** — Map out a website's hierarchy to understand site depth and page distribution instantly.
- **Execution Management** — List and delete crawl jobs to maintain strict organizational control over your scraping tasks.
- **Format Customization** — Retrieve data in markdown or HTML formats optimized for different LLM requirements.

### How it works

1. Subscribe to this server
2. Enter your Firecrawl API Key
3. Start managing your web extraction through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor website content and retrieve structured data straight from your workflow.
- **SEO Specialists** — verify website maps and page hierarchies without manual crawling.
- **Content Marketers** — perform rapid audits of competitor blogs and landing pages through natural language.
- **Growth Engineers** — automate web extraction querying to orchestrate cross-functional data teams smoothly.


## Available Tools
- **crawl_url**: Start a crawl job for a website
- **delete_crawl_job**: Delete a crawl job
- **get_crawl_status**: Get the status of a crawl job
- **list_crawl_jobs**: List all active and past crawl jobs
- **map_website**: Get a map of a website structure
- **scrape_url**: Scrape a single URL and return markdown


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Firecrawl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape https://vinkius.com/about and give me the markdown content."

**🤖 AI Agent:**
> I've scraped the page! I've retrieved the cleaned markdown which details Vinkius's mission and team. Would you like a summary of the core sections?

---

**👤 You:**
> "Start a crawl job for https://docs.firecrawl.dev with a limit of 10 pages."

**🤖 AI Agent:**
> Crawl job started! The Job ID is `job_12345`. I'll monitor the status for you. So far, it has identified the main documentation categories. Would you like me to notify you when it's done?

---

**👤 You:**
> "Map the website structure of https://github.com."

**🤖 AI Agent:**
> I've mapped out the hierarchy for GitHub. It includes major sections like /features, /pricing, and /trending. Would you like the full list of identified subdirectories?


## ❓ FAQ

**Q: How do I find my Firecrawl API Key?**
Log in to your [**Firecrawl.dev dashboard**](https://www.firecrawl.dev/app/settings/api-keys), and you will find your API Key under the settings. Copy and paste it below.

**Q: Can the agent crawl multiple pages at once?**
Yes. Use the `crawl_url` tool providing the base URL. Firecrawl will start a job to extract all subpages, and you can monitor the status via `get_crawl_status`.

**Q: Is it possible to see the website structure before scraping?**
Yes. The `map_website` tool allows your agent to retrieve a hierarchy of the site, giving you an audit of the structure before performing a full scrape or crawl.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firecrawl-alternative](https://vinkius.com/mcp/firecrawl-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Firecrawl** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `firecrawl-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Firecrawl** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firecrawl-alternative": {
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

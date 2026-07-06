# Browserhub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate web scraping via Browserhub — run scrapers, manage jobs, and retrieve extracted data directly from any AI agent.

## Description
Connect your **Browserhub.io** account to any AI agent and orchestrate your web scraping, data extraction, and proxy management workflows through natural conversation.

### What you can do

- **Scraper Oversight** — List all your configured scrapers and blueprints, and retrieve detailed metadata for each.
- **Job Execution** — Trigger scraping jobs with dynamic URL overrides and monitor their progress in real-time.
- **Direct Scraping** — Perform one-off URL extractions using real browsers without pre-defined scrapers.
- **Data Retrieval** — Retrieve structured data captured by your jobs directly into your workspace.
- **Infrastructure Management** — List available proxy locations and check your account credit balance.
- **Task History** — List and inspect all your previous scraping jobs.

### How it works

1. Subscribe to this server
2. Enter your Browserhub API Key
3. Start extracting data from any website from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Analysts** — quickly gather web data for datasets without manual scraper configuration.
- **Market Researchers** — monitor pricing or availability across multiple sites straight from their workflow tools.
- **Developers** — integrate web extraction and proxy rotation into their applications using natural language.


## Available Tools (10)
- **get_account_balance**: Check account credit balance
- **direct_scrape**: Perform a one-off URL scrape without a pre-defined scraper
- **get_blueprint**: Get details of a specific blueprint
- **get_scraping_job**: Get status and results of a scraping job
- **get_scraper**: Get details of a specific scraper
- **list_blueprints**: List all scraper blueprints
- **list_scraping_jobs**: List all scraping jobs
- **list_proxy_locations**: List all available proxy locations
- **list_scrapers**: List all configured scrapers
- **run_scraper**: Start a scraping job using a specific scraper


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browserhub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my configured scrapers in Browserhub."

**🤖 AI Agent:**
> I've retrieved your scrapers. You have 3 active configurations: 'E-commerce Prices' (ID: scr_1), 'News Articles' (ID: scr_2), and 'Lead Generator' (ID: scr_3).

---

**👤 You:**
> "Scrape the URL https://example.com using the 'E-commerce' scraper."

**🤖 AI Agent:**
> Scraping job job_99283 has been started for https://example.com. I will monitor it and notify you when the data is extracted.

---

**👤 You:**
> "Check my Browserhub account credit balance."

**🤖 AI Agent:**
> You currently have 1,500 credits remaining in your Browserhub account. This is enough for approximately 150-200 standard scrape requests.


## ❓ FAQ

**Q: Can I scrape a URL directly without creating a scraper first?**
Yes! Use the `direct_scrape` tool and provide the URL. It will use Browserhub's real browsers to render the page and extract data based on your parameters instantly.

**Q: How do I monitor the progress of a scraping job?**
Simply ask the agent to `get_scraping_job` and provide the Job ID. It will return the current status (e.g., pending, running, finished) and the result data once ready.

**Q: Can I specify a proxy location for my scraping request?**
Yes. When using `direct_scrape`, you can provide a `proxy_country` code. Use the `list_proxy_locations` tool to see the full list of supported countries in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserhub](https://vinkius.com/mcp/browserhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Browserhub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `browserhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Browserhub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "browserhub": {
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

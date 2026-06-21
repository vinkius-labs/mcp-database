# Bright Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bright-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access the world's #1 web data platform — bypass anti-bot protections, extract structured search engine data, and manage scraping browsers directly from your AI agent.

## Description
Connect your **Bright Data** account to any AI agent to automate complex web data extraction, bypass sophisticated anti-bot systems, and manage your proxy infrastructure through natural language.

### What you can do

- **Web Unlocking & SERP** — Use the `send_request` tool to bypass anti-bot protections or extract structured data from search engines using Web Unlocker or SERP API zones.
- **Dataset Orchestration** — Trigger large-scale data collections with `trigger_dataset`, monitor progress with `get_dataset_progress`, and download snapshots once ready.
- **Browser Management** — List and monitor active Scraping Browser sessions to debug or track automated browser workflows.
- **Infrastructure Control** — Retrieve all configured zones, check account status, and fetch proxy credentials (passwords) for specific zones securely.
- **Marketplace Discovery** — Browse available datasets in the Bright Data marketplace to find pre-collected data for your industry.

### How it works

1. Subscribe to this server
2. Enter your Bright Data API Key
3. Start scraping and managing proxies from Claude, Cursor, or any MCP-compatible client

Your AI now acts as a data engineer, capable of retrieving real-time web information even from the most protected sources.

### Who is this for?

- **Data Scientists & Analysts** — Automate the collection of training data or market intelligence without manual script execution.
- **Developers** — Debug scraping browser sessions and manage proxy zones directly from the code editor.
- **Market Researchers** — Extract structured SERP data to track rankings and competitor movements via simple conversation.


## Available Tools
- **get_all_zones**: Get all zones
- **get_dataset_progress**: Monitor dataset snapshot progress
- **get_dataset_snapshot**: Download a dataset snapshot
- **get_account_status**: Check account status
- **get_zone_info**: Get specific zone info
- **get_zone_passwords**: Get zone passwords
- **list_browser_sessions**: List Scraping Browser sessions
- **list_datasets**: List available datasets in the marketplace
- **send_request**: Send a request to Unlocker or SERP API
- **trigger_dataset**: Trigger a dataset collection (Crawl API)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bright Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active proxy zones in Bright Data."

**🤖 AI Agent:**
> I've retrieved your zones. You have 3 active zones: 'web_unlocker1' (Web Unlocker), 'serp_api_main' (SERP API), and 'residential_zone' (Residential Proxies).

---

**👤 You:**
> "Scrape the search results for 'best laptops 2024' using the SERP API zone."

**🤖 AI Agent:**
> Sending request to SERP API... I've extracted the structured data. The top results include reviews from TechRadar, CNET, and RTINGS. Would you like the full JSON output?

---

**👤 You:**
> "Check the progress of dataset snapshot 's_l1m2n3b4'."

**🤖 AI Agent:**
> The snapshot 's_l1m2n3b4' is currently at 75% completion. It has processed 15,000 records so far with 0 errors.


## ❓ FAQ

**Q: How do I bypass anti-bot systems on a specific website?**
Use the `send_request` tool and specify a zone configured with Web Unlocker. Provide the target URL, and Bright Data will handle the rotation and headers to return the content.

**Q: Can I check if my data collection is finished?**
Yes. Use the `get_dataset_progress` tool with your Snapshot ID. It will return the current percentage and status of the extraction process.

**Q: How do I get the proxy credentials for my scraper?**
You can use the `get_zone_passwords` tool by providing the zone name. This will retrieve the necessary passwords for proxy authentication.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bright-data](https://vinkius.com/mcp/bright-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bright Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bright-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bright Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bright-data": {
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

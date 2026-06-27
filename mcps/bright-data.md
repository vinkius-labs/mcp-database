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


## Available Tools (10)
- **get_dataset_snapshot**: Returns structured JSON records. Error records include error_code: "dead_page" (404) or "bad_input" (wrong URL pattern).

Download scraped data from a completed collection
- **trigger_dataset**: Poll get_dataset_progress until status="ready", then call get_dataset_snapshot to download results. Provide either url or keyword. LinkedIn Posts (gd_lyy3tktm25m4avu764) requires URLs matching linkedin.com/(pulse|posts|feed/update) — no keyword support. Always set include_errors=true.

Start an async scraping job for LinkedIn, Amazon, Instagram, and 100+ sources
- **get_zone_passwords**: For direct proxy connections outside this MCP. SENSITIVE — do not log credentials.

Get proxy credentials for direct connections (Selenium, Playwright, etc.)
- **list_browser_sessions**: Only relevant if Scraping Browser zones are configured. Default: 50 most recent.

List Scraping Browser sessions by status, duration, or bandwidth
- **get_account_status**: Use first if other tools return auth errors.

Check account status and API key validity
- **get_zone_info**: Use to verify a zone is active and correctly configured before using send_request.

Get zone configuration — type, status, bandwidth, and settings
- **list_datasets**: Use to find the correct dataset_id for trigger_dataset. Large response — filter by name.

Browse all 100+ available datasets with IDs and names
- **get_all_zones**: Call this before send_request to get valid zone names. Empty list means zones must be created at brightdata.com/cp/zones.

List all proxy zones configured in the account
- **get_dataset_progress**: Returns status ("running" or "ready"), records count, and errors count. Poll every 15-30s. Only call get_dataset_snapshot after status="ready". LinkedIn scraping takes 60-120s per URL.

Check if a dataset collection is complete
- **send_request**: Requires a valid zone name — call get_all_zones first if unknown. Web Unlocker zones scrape any site; SERP API zones return structured search results from Google/Bing URLs.

Scrape any URL bypassing anti-bot protections, or extract structured SERP data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bright Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape this LinkedIn post and extract the engagement data."

**🤖 AI Agent:**
> I triggered the LinkedIn Posts dataset with your URL and received snapshot `sd_abc123`. After polling for 90 seconds, the collection completed with 1 record and 0 errors. The post has 142 reactions, 23 comments, and was published 3 days ago. Here is the full structured data.

---

**👤 You:**
> "What proxy zones do I have available, and scrape this protected page."

**🤖 AI Agent:**
> You have 2 active zones: `web_unlocker1` (Web Unlocker) and `serp_api1` (SERP API). I used `web_unlocker1` to scrape the protected page and retrieved the full HTML content converted to markdown. The page contains 3 product listings with prices and reviews.

---

**👤 You:**
> "Find all available LinkedIn-related datasets I can use."

**🤖 AI Agent:**
> I found 6 LinkedIn datasets: LinkedIn Posts (`gd_lyy3tktm25m4avu764`), LinkedIn People Profiles (`gd_l1viktl72bvl7bjuj0` — 115M profiles), LinkedIn Companies (`gd_l1vikfnt1wgvvqz95w` — 55M companies), LinkedIn People Enriched (`gd_me5ppxjr2ge6icjuh0`), LinkedIn Companies with Jobs (`gd_mhf4aje023ctc3yn7w`), and LinkedIn Profiles by Position (`gd_la9vypp0jzg1bhkv3`). Which one would you like to use?


## ❓ FAQ

**Q: What is the workflow for scraping a LinkedIn post?**
Use `trigger_dataset` with the LinkedIn Posts dataset ID (`gd_lyy3tktm25m4avu764`) and a direct post URL (e.g., `https://www.linkedin.com/feed/update/urn:li:activity:...`). This returns a `snapshot_id`. Then poll `get_dataset_progress` every 15–30 seconds until the status is `ready` — LinkedIn scraping typically takes 60–120 seconds. Finally, call `get_dataset_snapshot` to retrieve the structured data including post content, author details, reactions, and comment count.

**Q: Why does send_request fail with a zone error?**
The `send_request` tool requires an active proxy zone (Web Unlocker or SERP API). If your account has no zones configured, the request will fail. Run `get_all_zones` first to check your available zones. If the list is empty, you need to create a zone in the [Bright Data dashboard](https://brightdata.com/cp/zones) before using `send_request`.

**Q: Which URL formats does the LinkedIn Posts dataset accept?**
The LinkedIn Posts dataset (`gd_lyy3tktm25m4avu764`) only accepts direct post URLs matching the pattern `linkedin.com/(pulse|posts|feed/update)`. Valid examples: `https://www.linkedin.com/feed/update/urn:li:activity:1234567890` or `https://www.linkedin.com/posts/username_title-activity-1234567890`. Search result pages, profile pages, and hashtag pages are not supported.

**Q: How do I find the right dataset ID for my use case?**
Use the `list_datasets` tool to browse all 100+ available datasets. Common IDs: LinkedIn Posts (`gd_lyy3tktm25m4avu764`), LinkedIn People (`gd_l1viktl72bvl7bjuj0`), LinkedIn Companies (`gd_l1vikfnt1wgvvqz95w`), Amazon Products (`gd_l7q7dkf244hwjntr0`), Instagram Profiles (`gd_l1vikfch901nx3by4`), Google Maps (`gd_m8ebnr0q2qlklc02fz`).


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
3. Set Type to "SSE" (or "streamable HTTP"), enter `bright-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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

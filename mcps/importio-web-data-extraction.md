# Import.io (Web Data Extraction) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/importio-web-data-extraction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extract structured data from any website via Import.io — run extractors, manage bulk crawls, and monitor API usage.

## Description
Connect your **Import.io** account to any AI agent and take full control of your web data extraction and large-scale scraping through natural conversation.

### What you can do

- **Precision Extraction** — Trigger predefined extractors for specific URLs to retrieve clean, structured JSON data directly from your agent
- **Bulk Crawling** — Start large-scale data extraction jobs across multiple pages concurrently using managed crawlers and monitor their progress in real-time
- **AI-Powered Magic API** — Automatically identify and extract tabular data from any website without pre-configured extractors, perfect for rapid exploration
- **Status Monitoring** — Poll ongoing extraction runs and crawl jobs to track processing states, success rates, and total pages processed
- **Data Export** — Retrieve extraction results in structured JSON or CSV formats, ready for spreadsheet processing or downstream application logic
- **Usage Audit** — Monitor your monthly API credit consumption and subscription limits to manage your data extraction budget effectively

### How it works

1. Subscribe to this server
2. Enter your Import.io API Key
3. Start extracting web data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — automate the collection of market data and pricing intelligence through natural conversation
- **Market Researchers** — perform large-scale competitor monitoring and web audits without manual scraping scripts
- **Product Managers** — verify data extraction schemas and monitor crawler health across multiple projects efficiently


## Available Tools
- **get_crawl_data**: Retrieve the unified JSON output of a completed import.io crawl job
- **get_crawl_status**: start_crawl to check progress (pages processed, success rate, current state).

Check the status of an ongoing import.io crawl job
- **download_csv**: Returns the first 1000 characters and file stats. Ideal for spreadsheet processing.

Download extraction data directly as CSV text
- **get_extractor_data**: Fails if the run is still in progress.

Retrieve structured JSON data from a completed import.io extraction
- **list_extractors**: Useful for finding the correct extractor_id to run dynamically.

List all extractors configured on the import.io account
- **run_magic_api**: Ideal for quick, unstructured exploration.

Run the import.io automated Magic API against a URL
- **run_extractor**: Triggers an async extraction run and returns a run_id. Use this run_id to poll for status or data.

Trigger an import.io extractor for a specific URL
- **start_crawl**: Starts a large-scale data extraction job across multiple pages concurrently.

Trigger an import.io bulk crawl job
- **get_extractor_status**: run_extractor. Returns the current state (running, completed, failed) and metadata about the run.

Check the status of an active or past import.io extraction run
- **account_usage**: No parameters required.

Check import.io account API credit usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Import.io (Web Data Extraction)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run extractor 'ext-123' against 'https://example.com/products'"

**🤖 AI Agent:**
> Extraction run started. Run ID: 'run-98765'. I'll monitor the status for you. It usually takes a few seconds to process dynamic pages. Would you like me to fetch the results once it's completed?

---

**👤 You:**
> "List all extractors in my Import.io account"

**🤖 AI Agent:**
> I've found 5 extractors in your account: 'Amazon Scraper' (ext-001), 'Competitor Pricing' (ext-002), 'Real Estate Leads' (ext-003), 'Stock Tracker' (ext-004), and 'News Monitor' (ext-005). Which one would you like to run?

---

**👤 You:**
> "Check my monthly API credit usage"

**🤖 AI Agent:**
> You've used 12,450 credits out of your 50,000 monthly limit (24.9%). You have 37,550 credits remaining for this billing cycle. Your account health is excellent.


## ❓ FAQ

**Q: Can I extract data from a website without a pre-configured extractor?**
Yes. Use the `run_magic_api` tool. It uses Import.io's AI logic to automatically detect and extract structured or tabular data from any URL, making it ideal for quick exploration of new data sources.

**Q: How do I monitor the progress of a bulk crawl job?**
Use the `get_crawl_status` tool by providing the Crawl ID returned when you started the job. Your agent will report the current state, number of pages processed, and success rate in real-time.

**Q: Can I get my extracted data in CSV format for spreadsheet analysis?**
Absolutely. Use the `download_csv` tool with a completed Run ID. Your agent will retrieve the extraction data in CSV format, perfect for processing in tools like Excel or Google Sheets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/importio-web-data-extraction](https://vinkius.com/mcp/importio-web-data-extraction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Import.io (Web Data Extraction)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `importio-web-data-extraction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Import.io (Web Data Extraction)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "importio-web-data-extraction": {
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

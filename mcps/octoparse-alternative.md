# Octoparse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/octoparse-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Scrape data from any website visually with a no-code web scraper that handles pagination, login, and JavaScript rendering.

## Description
Connect your **Octoparse** account to any AI agent and take full control of your web data orchestration through natural conversation. Octoparse is the premier no-code web scraping tool, and this integration allows you to retrieve task metadata, trigger cloud extractions, and ingest structured web data directly from your chat interface.

### What you can do

- **Task & Group Orchestration** — List all managed scraping tasks and retrieve detailed group metadata programmatically to ensure your data foundation is always synchronized.
- **Cloud Extraction Control** — Start and stop cloud-based scraping tasks directly from the AI interface to rapidly gather real-time data from any website.
- **Extraction Intelligence** — Retrieve extracted data in bulk or filter for 'non-exported' records via natural language to drive better research efficiency.
- **Status Monitoring Oversight** — Access real-time task statuses (Running, Completed, Stopped) using simple AI commands to ensure your data collection is always optimized.
- **Operational Monitoring** — Track system responses and manage data status updates to maintain a high-fidelity interaction history.

### How it works

1. Subscribe to this server
2. Enter your Octoparse OpenAPI Access Token from your profile settings
3. Start managing your web scrapers from Claude, Cursor, or any MCP-compatible client

No more manual exporting of CSV results for basic checks. Your AI acts as a dedicated data researcher or extraction lead.

### Who is this for?

- **Market Researchers** — quickly retrieve competitor data and monitor pricing trends without switching apps.
- **Data Analysts** — automate the ingestion of web data and track extraction health via natural conversation.
- **Developers** — integrate real-time web scraping and data retrieval directly within the chat.


## Available Tools (8)
- **get_new_data**: Get new (non-exported) data from a task
- **get_task_data**: Get extracted data from a task by offset
- **get_task_status**: Get status of a scraping task
- **list_task_groups**: List all task groups
- **list_tasks**: Can be filtered by task group ID.

List tasks
- **start_task**: Start a scraping task
- **stop_task**: Stop a scraping task
- **update_data_status**: Mark data as exported


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Octoparse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my scraping tasks in Octoparse."

**🤖 AI Agent:**
> I've retrieved your tasks. You have 5 active scrapers including 'Amazon Monitor' and 'Real Estate Leads'. Which one would you like to start or retrieve data for?

---

**👤 You:**
> "Start running my Amazon product scraping task and check its current status."

**🤖 AI Agent:**
> Task "Amazon Electronics Scraper" (ID: tsk_8921) has been started successfully. Current status: Running. It is processing page 12 of an estimated 85 pages. 264 product records have been extracted so far. Estimated completion: approximately 45 minutes based on current crawl speed.

---

**👤 You:**
> "Get the extracted data from my latest completed scraping task."

**🤖 AI Agent:**
> Fetching results from task "Competitor Pricing Monitor" (ID: tsk_8905), completed 3 hours ago. Retrieved 1,247 records with fields: Product Name, Price, Rating, Review Count, and URL. The first batch of 100 records is ready. Shall I export the full dataset or retrieve the next page of results?


## ❓ FAQ

**Q: Can my AI automatically find the latest extracted data for a specific task?**
Yes! Use the `get_not_exported_data` tool with the Task ID. Your agent will respond with complete metadata for the newest records that haven't been marked as exported yet in seconds.

**Q: How do I find my Octoparse OpenAPI Access Token?**
Log in to Octoparse, navigate to the **OpenAPI** section in your profile or developer portal, and follow the instructions to generate a Bearer token using your account credentials.

**Q: Can I start a scraper via the AI?**
Absolutely. Use the `start_task` tool with your Task ID. The AI will command Octoparse to begin the extraction in the cloud immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/octoparse-alternative](https://vinkius.com/mcp/octoparse-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Octoparse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `octoparse-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Octoparse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "octoparse-alternative": {
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

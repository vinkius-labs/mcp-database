# Browse AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browse-ai-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate web scraping with Browse AI — run extraction robots, monitor page changes, and retrieve bulk data directly from any AI agent.

## Description
Connect your **Browse AI** account to any AI agent and take full control of your no-code web scraping operations through natural conversation.

### What you can do

- **Robot Discovery** — List all your trained extraction and monitoring robots along with their configuration details
- **Execute Scrapes** — Trigger specific robots to run tasks on target URLs without lifting a finger
- **Data Retrieval** — Instantly download the final extracted JSON data from any successfully completed task
- **Bulk Operations** — Initiate multi-URL concurrent extractions and download the unified bulk datasets
- **Monitor Sync** — Check the status of your active web change monitors
- **Quota Management** — Retrieve your current API credits usage and monthly plan limits

### How it works

1. Subscribe to this server
2. Enter your Browse AI Secret API Key
3. Start fetching live data via Claude, Cursor, or any MCP-compatible client

No more manual downloads or periodic checks. Your AI agent serves as your pipeline to live web intelligence.

### Who is this for?

- **Data analysts** — pull massive datasets from recent bulk tasks straight into your agent for immediate processing
- **Marketers & SEO** — execute scraping robots on competitor URLs to generate instant market reports
- **Researchers** — extract complex targeted metrics without opening any third-party dashboards
- **Developers** — verify robot configurations, monitor credit usage, and inspect JSON payloads rapidly


## Available Tools
- **run_bulk_task**: Each set typically contains a different "originUrl". All extractions run concurrently on Browse AI infrastructure.

Run a Browse AI robot in bulk mode across multiple URLs
- **download_bulk_data**: Returns a JSON array where each element contains the capturedData from one task.

Download all extracted results from a completed Browse AI bulk run
- **get_bulk_task**: Get bulk task execution status from Browse AI
- **get_robot**: Get detailed configuration of a specific Browse AI robot
- **get_task_data**: Only meaningful when the task status is "successful". Fields match the column names configured in the Browse AI robot builder hitting internal task references.

Retrieve the final extracted JSON data from a successful Browse AI task
- **get_task**: Check the status of a specific Browse AI extraction task
- **list_credits**: Check Browse AI quota limits and credit usage
- **list_monitors**: Monitors run on scheduled intervals to detect changes on target web pages and trigger notifications or data captures automatically via `/monitors`.

List all active Browse AI web monitoring robots
- **list_robots**: Each robot represents a no-code AI scraping workflow targeting a specific website or data pattern via `GET /robots`.

List all Browse AI extraction and monitoring robots
- **run_robot**: Pass a JSON string of input parameters (typically including "originUrl" for the target page and any variable fields the robot expects). Returns a taskId.

Trigger a Browse AI robot to extract data from a target URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browse AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my robots. Which ones are built for monitoring?"

**🤖 AI Agent:**
> You have 3 robots active. 
1. [a0f2b] 'Competitor Price Tracker' 
2. [h6j2x] 'HackerNews Scraper'
3. [k9b1a] 'Amazon Search Result Extractor'. 
By cross-referencing with your monitors list, the 'Competitor Price Tracker' is your only robot currently running on an automated monitoring schedule.

---

**👤 You:**
> "Run my HackerNews Scraper robot on the main page."

**🤖 AI Agent:**
> Task started successfully! The new Task ID is `t-78ab31`. The robot [h6j2x] is currently capturing data. Once it finishes, I can retrieve the articles for you. Would you like me to check its status now?

---

**👤 You:**
> "Retrieve the JSON data for task t-78ab31."

**🤖 AI Agent:**
> The task completed successfully. Here is the extracted data (Top 3 items):
1. "OpenAI Announces New Models" (URL: https://news.ycombinator.com/item?id=...)
2. "Show HN: A new programming language" (URL: ...)
3. "React 19 Release Notes" (URL: ...)

I have the full JSON array stored in context if you want to perform deep filtering on the other 27 scraped items.


## ❓ FAQ

**Q: Can my AI start a data extraction and let me know when it finishes?**
Yes! You can ask your agent to `run_robot` on a certain URL. The agent receives the newly created task ID and can immediately invoke `get_task` sequentially to poll for completion. Once successful, it calls `get_task_data` to dump the JSON right into your conversation without breaking workflow.

**Q: How do bulk operations work natively through the agent?**
When you have a trained robot, you can feed the `run_bulk_task` command an array of different URLs. Browse AI's backend splits them virtually into independent task instances. Your agent tracks the bulk run via `get_bulk_task` and eventually pulls the mega JSON merge using `download_bulk_data`.

**Q: Is there a risk of my agent suddenly spending all my API credits?**
You have complete visibility—the agent can query `list_credits` at any moment to inform you precisely of your available balance and monthly limit. Also, since tools execute your natural directives, your AI agent only triggers extractions you specifically prompt for.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browse-ai-1](https://vinkius.com/mcp/browse-ai-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Browse AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `browse-ai-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Browse AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "browse-ai-1": {
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

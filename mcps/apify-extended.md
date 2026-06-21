# Apify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apify-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Run web scraping actors, collect structured data, and manage storage datasets for large-scale data extraction projects.

## Description
Connect your **Apify** account to any AI agent and simplify how you manage your web scraping, automation actors, and data storage through natural conversation.

### What you can do

- **Actor Control** — List and trigger serverless actors for web scraping and automation directly from your agent.
- **Dataset Retrieval** — Fetch the resulting data records (items) from your datasets to analyze or process values via AI.
- **Run Monitoring** — Track the history and status of recent actor executions to ensure reliability.
- **Task Management** — List and query configured actor tasks to reuse saved scraper settings.
- **Data Insights** — Retrieve detailed metadata and logs for specific runs to debug complex automations.
- **Storage Visibility** — List all datasets in your account to manage your collected web data.

### How it works

1. Subscribe to this server
2. Enter your Apify API Token (found in your account settings under Integrations)
3. Start running your scrapers from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Scientists & Researchers** — quickly retrieve scraped data from datasets and analyze trends via simple AI commands.
- **Automation Engineers** — trigger actor runs and monitor execution health directly from the workspace.
- **Product Managers** — get instant bird's-eye views of automated data collection tasks and results.


## Available Tools (7)
- **get_dataset_results**: Get items from a dataset
- **get_run_details**: Get details for a specific run
- **list_actors**: List Apify actors
- **list_datasets**: List Apify datasets
- **list_actor_runs**: List recent actor executions
- **list_actor_tasks**: List configured actor tasks
- **run_actor**: Trigger an actor run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all actors in my Apify account."

**🤖 AI Agent:**
> I've retrieved your actors. You have 3 active scrapers including 'Instagram Scraper', 'Google Maps Reviewer', and 'Custom CRM Sync'. Which one would you like to run or check datasets for?

---

**👤 You:**
> "Run the 'Instagram Scraper' with input { "hashtags": ["#AI"] }."

**🤖 AI Agent:**
> Actor run triggered! I've started the 'Instagram Scraper' (ID: act_10293) with your custom input. The execution ID is run_88231. I'll monitor it and let you know when the dataset is ready.

---

**👤 You:**
> "Show me the results from dataset 'ds_10293'."

**🤖 AI Agent:**
> I've fetched the dataset items. There are 25 records including profile URLs, post captions, and engagement counts. Would you like me to summarize the top performing posts?


## ❓ FAQ

**Q: Can I provide input parameters when running an actor?**
Yes! Use the `run_actor` tool and provide the optional `input` JSON object to configure specific scraper settings for that run.

**Q: How do I see the items collected in a dataset?**
Run the `get_dataset_results` query with your Dataset ID. The agent will retrieve the data records, which you can then ask the AI to summarize or analyze.

**Q: Is it possible to check the status of a specific actor run?**
Absolutely. Use the `get_run_details` tool and provide the Run ID. Your agent will retrieve the status (RUNNING, SUCCEEDED, FAILED) and metadata for that specific execution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apify-extended](https://vinkius.com/mcp/apify-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apify-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apify-extended": {
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

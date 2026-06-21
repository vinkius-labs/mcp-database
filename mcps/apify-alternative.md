# Apify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apify-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Manage your cloud automation — audit actors, tasks, and datasets via AI.

## Description
Empower your AI agent to orchestrate your entire cloud automation and web scraping ecosystem with **Apify**, the leading platform for scaleable automation. By connecting Apify to your agent, you transform complex actor management into a natural conversation. Your agent can instantly list your actors, audit task execution, and retrieve dataset items without you ever touching a technical console. Whether you are running data pipelines or managing automated workflows, your agent acts as a real-time automation operator, ensuring your cloud jobs are always monitored and your data is organized.

### What you can do

- **Actor Auditing** — List all actors in your account and retrieve detailed metadata, including descriptions and status.
- **Task Oversight** — Browse your configured actor tasks to maintain a clear view of your automated workflows.
- **Execution Intelligence** — List recent runs for any actor or task to monitor performance and success rates in real-time.
- **Data Management** — Query datasets and retrieve items instantly to audit the output of your automation jobs.
- **Operational Monitoring** — List schedules, webhooks, and key-value stores to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Apify API Key
3. Start managing your cloud automation through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor actor runs and dataset items straight from your workflow.
- **Operations Managers** — verify if automated tasks are being correctly executed and scheduled.
- **Growth Leads** — perform rapid audits of scraping outputs and extracted data without manual logins.
- **Business Owners** — automate cloud querying to orchestrate your data-driven automation strategy smoothly.


## Available Tools
- **list_webhooks**: List configured webhooks
- **get_actor**: Get details for a specific actor
- **get_dataset_items**: Get items from a specific dataset
- **get_user_info**: Get details for the authenticated Apify user
- **list_actors**: List Apify actors
- **list_datasets**: List Apify datasets
- **list_key_value_stores**: List Apify key-value stores
- **list_runs**: List runs for an actor
- **list_schedules**: List Apify schedules
- **list_tasks**: List Apify actor tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Apify actors."

**🤖 AI Agent:**
> I've retrieved your actors. You have 5 active actors, including 'Website Content Crawler' and 'Google Maps Scraper'. Which one would you like to audit for recent runs?

---

**👤 You:**
> "Show me the last 5 runs for actor ID xxxx."

**🤖 AI Agent:**
> I've found the last 5 runs. The most recent one was completed successfully in 2 minutes. Two other runs had warnings. Would you like the full log details?

---

**👤 You:**
> "Get items from dataset ID yyyy."

**🤖 AI Agent:**
> I've retrieved the data from that dataset. It contains 50 items related to 'Competitor Pricing'. I can summarize the top findings or provide the full list.


## ❓ FAQ

**Q: How do I find my Apify API Key?**
Log in to your [**Apify Console**](https://console.apify.com/account/integrations), and you will find your API Token under the **Integrations** tab. Copy and paste it below.

**Q: Can the agent check the results of a scrape?**
Yes. Use the `get_dataset_items` tool providing the Dataset ID. Your agent will retrieve the items from the cloud storage, allowing you to audit the output instantly.

**Q: Is it possible to list actor runs via the agent?**
Yes. The `list_runs` tool allows your agent to retrieve the history of executions for any specific actor, including durations and final statuses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apify-alternative](https://vinkius.com/mcp/apify-alternative)
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
3. Set Type to "SSE", enter `apify-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apify-alternative": {
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

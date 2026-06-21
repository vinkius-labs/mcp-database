# Octoparse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/octoparse)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI agent to Octoparse to trigger cloud web scraping tasks, monitor crawler statuses, and retrieve scraped data directly into chat.

## Description
Connect your **Octoparse** framework to your AI agent and turn cloud-based web scraping into a fully conversational command center.

### What you can do

- **Task Execution** — Trigger the launch engine using `start_task` whenever data refresh is needed, or invoke `stop_task` to halt runaway crawlers instantly.
- **Status Monitoring** — Keep a pulse on active bots by calling `get_task_status`, or systematically drill down through your project taxonomy via `list_task_groups` and `list_tasks`.
- **Data Ingestion** — Dump the latest extracted web rows natively into the AI's context using `get_task_data`, allowing the LLM to format, structure, or summarize the results immediately.
- **Token Operations** — Authenticate dynamically utilizing `get_token` with your core credentials.

### How it works

1. Subscribe to this server
2. Enter your Premium Octoparse API Credentials (Username/Email and Password)
3. Command your agent (e.g., Claude or Cursor) to spin up scrapers and read the downloaded data directly onto your IDE

### Who is this for?

- **Data Engineers** — trigger scheduled pipelines, check extraction states, and dump JSON samples to debug schemas without leaving your terminal.
- **Growth Hackers** — quickly spin up an Amazon or LinkedIn scraper, grab the extracted table data, and have the AI formulate email lists simultaneously.
- **Business Analysts** — fetch the competitive pricing matrices scraped overnight and ask the AI to summarize price drops directly in the conversation.


## Available Tools
- **clear_task_data**: Done to purge testing footprints before production crawls.

Delete all securely stored data for an Octoparse task
- **get_task_data**: Use offset-based pagination strictly to prevent memory crash exceptions (max 1000 limit).

Export un-exported data from a completed Octoparse scraping task
- **get_task_status**: Get the current running status of an Octoparse cloud task
- **get_token**: 0 password grant. Returns an access_token. The access_token must be stored and reused for API calls until expiration.

Obtain an OAuth 2.0 access token from Octoparse
- **list_task_groups**: Use these IDs to filter executing scraping tasks nested inside a specific folder limit.

List all task groups (folders) in the Octoparse account
- **list_tasks**: Each task includes a taskId, status, and creation date. Use the taskId for starting or polling data.

List all configured cloud scraping tasks on Octoparse
- **mark_data_exported**: Execute this immediately after a successful `get_task_data`.

Mark all currently stored data in an Octoparse task as extracted
- **start_task**: Task changes status to Running instantly.

Start a cloud scraping task on Octoparse
- **stop_task**: Stop a running Octoparse cloud task
- **update_task_params**: g. changing the core search URL or injected keywords) without opening the Octoparse IDE cleanly scaling parameterized bots.

Dynamically update URL or parameter constraints driving a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Octoparse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up task 'LinkedIn Profiles Q4' and tell me how many rows it extracted."

**🤖 AI Agent:**
> The Cloud Agent confirms the task 'LinkedIn Profiles Q4' finished running successfully and acquired `4523` rows of active data.

---

**👤 You:**
> "Start my Amazon Price Monitor crawler task now."

**🤖 AI Agent:**
> Task started. Your 'Amazon Price Monitor' has been queued to the cloud servers and will begin fetching targeted DOM elements shortly.

---

**👤 You:**
> "Get the data extracted from task 'Real Estate NYC' and format it as a markdown table."

**🤖 AI Agent:**
> I've fetched the rows successfully. Here is the structured breakdown highlighting the `Address`, `Square Footage`, `Beds`, and estimated `Asking Price`...


## ❓ FAQ

**Q: Can I have my AI format the scraped JSON into a clean Markdown table?**
Absolutely. Because Octoparse MCP connects natively via the `get_task_data` capability directly into the AI's isolated context window, the language model can instantly translate cumbersome JSON fields into polished, structured, and legible tabular outputs on demand.

**Q: Is it possible to track task progress percentage in the chat?**
Yes. When you instruct your agent to run `get_task_status`, it fetches the real-time runtime progress metrics from Octoparse's cloud. You'll see whether it's Waiting, Running, or Completed, along with how many rows have been extracted so far.

**Q: Do I need a paid Octoparse plan for API capabilities to work?**
Yes. Octoparse explicitly limits their Advanced Cloud APIs strictly to their paid subscription levels. A Free tier account will reject the authentication tokens when attempting to fetch the runtime data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/octoparse](https://vinkius.com/mcp/octoparse)
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
3. Set Type to "SSE", enter `octoparse` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Octoparse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "octoparse": {
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

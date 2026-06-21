# Browserbear MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserbear)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate browser tasks via Browserbear — take screenshots, scrape data, and run multi-step automations directly from any AI agent.

## Description
Connect your **Browserbear (Roborabbit)** account to any AI agent and orchestrate your browser automation, web scraping, and visual monitoring workflows through natural conversation.

### What you can do

- **Task Oversight** — List and retrieve detailed metadata for all your saved browser automation tasks.
- **Automation Execution** — Trigger task runs with dynamic overrides (like URL or form data) and monitor their progress.
- **Visual Captures** — Take high-quality screenshots of any URL with customizable dimensions and wait times.
- **Data Extraction** — Retrieve scraped structured data and screenshot URLs directly into your workspace.
- **Run Management** — List, inspect, and delete history of your automation runs.
- **Project Coordination** — Access and organize your tasks across multiple projects and track account usage.

### How it works

1. Subscribe to this server
2. Enter your Browserbear API Key
3. Start automating the web from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — quickly trigger visual regression tests and inspect results without manual dashboard work.
- **Growth Marketers** — automate lead gathering or competitor monitoring straight from their workflow tools.
- **Developers** — integrate complex browser interactions into their coding environment using natural language.


## Available Tools
- **create_task**: Create a new browser automation task
- **delete_run**: Delete a task run record
- **get_run**: Get status and results of a task run
- **get_task**: Get details of a specific task
- **get_account_usage**: Retrieve account usage statistics
- **list_projects**: List all projects in the account
- **list_runs**: List all task runs
- **list_tasks**: List all browser automation tasks
- **run_task**: Trigger a run for a specific task
- **take_screenshot**: Take a quick screenshot of a URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browserbear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my browser automation tasks."

**🤖 AI Agent:**
> I've retrieved your tasks. You have 3 tasks: 'Daily News Scraper' (ID: task_1), 'Visual Check' (ID: task_2), and 'Login Flow' (ID: task_3).

---

**👤 You:**
> "Take a screenshot of https://vinkius.com at 1280x800 resolution."

**🤖 AI Agent:**
> Screenshot run created! I'm capturing https://vinkius.com now. You can check the result using run ID run_99283 in a few moments.

---

**👤 You:**
> "Run task task_123 and override the starting URL to https://google.com."

**🤖 AI Agent:**
> Task run tr_8877 has been triggered with the URL override. I will monitor it for completion.


## ❓ FAQ

**Q: Can I trigger a browser task with a different starting URL?**
Yes! Use the `run_task` tool and provide the Task ID. In the `overrides` field, you can pass a JSON object like `{"url": "https://newsite.com"}` to change the starting point dynamically.

**Q: How do I see the screenshot captured by a task?**
Simply ask the agent to `get_run` and provide the Run ID. Once the status is 'finished', the response will include a `screenshot_url` that you can click to view the image.

**Q: Does the integration allow taking a quick screenshot without a saved task?**
Yes. Use the `take_screenshot` action and provide the URL. It will create a simplified run that captures the page and returns the result URL once processed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserbear](https://vinkius.com/mcp/browserbear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Browserbear** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `browserbear` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Browserbear** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "browserbear": {
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

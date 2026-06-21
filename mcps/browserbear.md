# Browserbear MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserbear)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browserbear-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browserbear-mcp)
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


## Installation & Usage

To install and use the **Browserbear** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserbear](https://vinkius.com/mcp/browserbear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Browse AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browse-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browse-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browse-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate web data extraction via Browse AI — run robots, monitor websites, and retrieve captured data directly from any AI agent.

## Description
Connect your **Browse AI** account to any AI agent and orchestrate your web scraping, data extraction, and website monitoring workflows through natural conversation.

### What you can do

- **Robot Oversight** — List all your approved robots and retrieve detailed metadata for each scraper.
- **Task Execution** — Trigger robot runs (tasks) on specific URLs and monitor their progress in real-time.
- **Data Retrieval** — Retrieve structured data captured by your robots directly into your workspace.
- **Website Monitoring** — List and create monitor schedules to track changes on any website automatically.
- **Bulk Operations** — Manage and inspect bulk runs to extract data from multiple sources at once.
- **System Status** — Check the health and queue status of the Browse AI infrastructure.

### How it works

1. Subscribe to this server
2. Enter your Browse AI Secret API Key
3. Start extracting web data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — quickly trigger data extractions and retrieve results without manual dashboard exports.
- **Growth Marketers** — monitor competitor prices or new listings straight from their workflow tools.
- **Developers** — integrate web extraction logic into their coding environment using natural language.


## Available Tools
- **create_monitor**: Create a new monitor schedule for a robot
- **get_bulk_run**: Get details of a specific bulk run
- **get_robot**: Get details of a specific robot
- **get_system_status**: Check Browse AI system and queue status
- **get_task**: Get status and extracted data for a task
- **list_bulk_runs**: List all bulk runs for a robot
- **list_monitors**: List all monitors for a specific robot
- **list_robots**: List all approved robots
- **list_tasks**: List all tasks for a specific robot
- **run_robot**: Run a robot to extract data (creates a task)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browse AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my approved web scraping robots."

**🤖 AI Agent:**
> I've retrieved your robots. You have 3 active robots: 'Amazon Price Tracker' (ID: rob_1), 'LinkedIn Lead Extractor' (ID: rob_2), and 'Real Estate Monitor' (ID: rob_3).

---

**👤 You:**
> "Run robot rob_123 on https://example.com/product."

**🤖 AI Agent:**
> Task created! Robot rob_123 is now processing the URL. You can check the progress and results using task ID task_998877.

---

**👤 You:**
> "Retrieve the data from task task_99283."

**🤖 AI Agent:**
> Task task_99283 is successful. Captured data includes: Product Name: 'Modern Lamp', Price: '$45.00', Stock: 'In Stock'. Would you like the full JSON?


## Installation & Usage

To install and use the **Browse AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browse-ai](https://vinkius.com/mcp/browse-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

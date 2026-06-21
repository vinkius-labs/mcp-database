# Browse AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browse-ai-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browse-ai-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browse-ai-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Extract data from any website without code using trained robots that monitor pages and deliver structured results automatically.

## Description
Connect your **Browse AI** account to any AI agent and take full control of your no-code web scraping and automated monitoring workflows through natural conversation.

### What you can do

- **Robot Orchestration** — List and manage all web scraping robots in your account programmatically, retrieving detailed configuration and high-fidelity extraction history
- **Automated Task Execution** — Programmatically trigger new robot runs with custom parameters (e.g., origin URL) to coordinate high-fidelity data collection in real-time
- **Website Monitoring Intelligence** — Create and manage monitoring schedules to track changes on any website and maintain a perfectly coordinated data pipeline
- **Event Architecture** — Access and monitor robot webhooks for instant notifications and retrieve detailed log metadata directly through your agent
- **Financial Visibility** — Programmatically track your account subscription status and credit usage to coordinate your automated data quotas efficiently

### How it works

1. Subscribe to this server
2. Retrieve your **Secret API Key** from your Browse AI dashboard (Account > API)
3. Start collecting web data and monitoring sites from Claude, Cursor, or any MCP client

No more manual logging into the dashboard to check individual extraction tasks. Your AI acts as your dedicated data engineer and monitoring coordinator.

### Who is this for?

- **Market Researchers** — instantly trigger price scraping and competitive monitoring using natural language commands
- **Growth Marketers** — automate lead generation from public directories and track site changes without leaving your workspace
- **Developers** — integrate high-speed no-code scraping data into custom workflows through simple AI queries


## Available Tools
- **create_monitor**: Add new schedule
- **remove_webhook**: Delete robot webhook
- **get_user_profile**: Get account info
- **get_robot_details**: Get robot info
- **get_usage_quotas**: Check credit balance
- **get_run_status**: Check task progress
- **list_bulk_operations**: List bulk task runs
- **list_active_monitors**: List scheduled scrapers
- **list_robots**: List scraping robots
- **list_robot_history**: List past runs
- **list_robot_webhooks**: Get event configs
- **trigger_robot_run**: Start scraping task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browse AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available scraping robots in my account."

**🤖 AI Agent:**
> I've retrieved your robots. You currently have 5 active scrapers, including 'Price Monitor' (ID: rob_123) and 'Lead Extractor'. Which one would you like to execute or inspect?

---

**👤 You:**
> "Trigger robot 'rob_123' to scrape 'https://vinkius.com/pricing'."

**🤖 AI Agent:**
> Scraping task triggered! I've initiated a new run for robot rob_123 with your custom URL. The task ID is 'task_456'. I'll monitor the progress and notify you once the results are ready.

---

**👤 You:**
> "Check the status and results for task 'task_456'."

**🤖 AI Agent:**
> Fetching results... Task task_456 has successfully 'Finished'. I've retrieved 12 data points including plan names and monthly prices. Would you like the full high-fidelity JSON export?


## Installation & Usage

To install and use the **Browse AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browse-ai-alternative](https://vinkius.com/mcp/browse-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

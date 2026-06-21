# Hexomatic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hexomatic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hexomatic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hexomatic-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate web scraping and worklfows via Hexomatic — manage workflows, recipes, and automation logs directly from any AI agent.

## Description
Connect your **Hexomatic** account to any AI agent and take full control of your web scraping and no-code automation workflows through natural conversation.

### What you can do

- **Workflow Oversight** — List all automation workflows, retrieve detailed configurations, and monitor their active status.
- **Run Automations** — Manually trigger workflow executions and pass runtime variables like target URLs directly from the chat.
- **Scraping Insights** — List point-and-click scraping recipes and retrieve output data from completed executions.
- **Execution Logs** — Access detailed logs for any workflow run to troubleshoot or audit automation steps.
- **Built-in Automations** — Browse 100+ ready-to-use automations, including Tech Stack Discovery and Email Finding.
- **Usage Monitoring** — Instantly check your account's automation credits and current plan usage.

### How it works

1. Subscribe to this server
2. Enter your Hexomatic API Key (found in Settings > API)
3. Start managing your automations from Claude, Cursor, or any MCP-compatible client

No more manual configuration in the web dashboard for every run. Your AI assistant acts as a dedicated Automation Architect or Data Scraping Specialist.

### Who is this for?

- **Growth Marketers** — instantly trigger lead generation workflows and retrieve enriched prospect lists.
- **Data Analysts** — automate the extraction of data from target websites and monitor scraping success rates.
- **Product Researchers** — use AI to analyze competitor tech stacks and news through automated workflows.


## Available Tools
- **get_workflow_results**: Retrieve the output data from a completed workflow execution
- **get_execution_logs**: Retrieve the execution logs for a specific workflow
- **get_account_usage**: Retrieve current plan usage and automation credits
- **get_workflow_details**: Get detailed configuration for a specific workflow
- **list_automations**: List all built-in Hexomatic automations (e.g., Tech Stack Discovery)
- **list_scraping_recipes**: List all point-and-click scraping recipes
- **list_account_teams**: List teams and collaborators
- **list_workflows**: Use this to identify the ID of the workflow you want to run.

List all automation workflows in your Hexomatic account
- **run_workflow**: You can pass runtime variables like input URLs as a JSON string in "body_json".

Manually trigger an execution of a workflow
- **search_workflows**: Search for workflows by name or title
- **update_workflow_status**: Activate or deactivate a workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hexomatic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active automation workflows."

**🤖 AI Agent:**
> I've retrieved your workflows. You have 4 active automations: 'Competitor Pricing Scraper', 'Tech Stack Discovery', 'LinkedIn Lead Finder', and 'Product News Tracker'. Which one would you like to run or inspect?

---

**👤 You:**
> "Show me the results from the latest 'Tech Stack Discovery' run."

**🤖 AI Agent:**
> Accessing workflow results... The latest run for 'Tech Stack Discovery' (ID: hex_992) found that 'example.com' uses AWS, React, and Intercom. 'target-app.io' uses Google Cloud and Vue.js. Should I export these results to a summary for you?

---

**👤 You:**
> "Run workflow ID 'hex_5501' with the target URL 'https://vinkius.com'."

**🤖 AI Agent:**
> Workflow triggered! I've successfully started the execution of workflow hex_5501 with the provided URL. You can check the progress using the `get_execution_logs` tool in a few minutes.


## Installation & Usage

To install and use the **Hexomatic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hexomatic](https://vinkius.com/mcp/hexomatic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

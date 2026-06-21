# YepCode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yepcode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yepcode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yepcode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Run serverless code snippets in the cloud with a platform that lets you build integrations and automations in any programming language.

## Description
Connect your **YepCode** account to any AI agent and simplify how you automate complex data integrations and serverless workflows through natural conversation.

### What you can do

- **Process Control** — List and trigger serverless processes with custom parameters directly from your agent.
- **Execution Monitoring** — Track the history and status of your workflow runs to ensure reliability.
- **Secret Management** — List and verify account secrets used in your automations without exposing values.
- **Team Coordination** — Query available teams and workspaces to understand your development environment.

### How it works

1. Subscribe to this server
2. Enter your YepCode API Key
3. Start running and monitoring your serverless automations from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — quickly trigger maintenance workflows or data syncs via simple AI commands.
- **Data Analysts** — monitor the status of recurring ETL processes and verify secret availability.
- **Software Developers** — test and run serverless functions during the development cycle without leaving the IDE.


## Available Tools
- **get_process_details**: Get details for a specific process
- **list_executions**: List recent process executions
- **list_processes**: List YepCode processes
- **list_secrets**: List account secrets
- **list_teams**: List available teams
- **run_process**: Trigger a process execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YepCode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available processes in my YepCode account."

**🤖 AI Agent:**
> I've retrieved your processes. You have 5 serverless workflows configured, including 'Database Sync', 'PDF Generator', and 'Slack Notifier'. Which one would you like to run?

---

**👤 You:**
> "Run the 'Data Export' process with the parameter { "format": "csv" }."

**🤖 AI Agent:**
> Process triggered! The 'Data Export' execution has started with ID exe_12930. I'll let you know when the history shows it's complete.

---

**👤 You:**
> "Check the status of my recent process executions."

**🤖 AI Agent:**
> Inspecting recent executions... I found 3 entries: 'PDF Generator' (Success), 'Database Sync' (Success), and 'Web Scraper' (Error). Would you like the error logs for the Web Scraper?


## Installation & Usage

To install and use the **YepCode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yepcode](https://vinkius.com/mcp/yepcode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

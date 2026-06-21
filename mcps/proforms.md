# Proforms MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/proforms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/proforms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/proforms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Online form builder and data collection.

## Description
The Proforms MCP server allows your AI agent to query form responses, retrieve submission data, and list active forms natively. Analyze your collected data immediately through conversation without downloading CSV files.


## Available Tools
- **create_job**: Push a new job to a field worker
- **get_asset**: Retrieve details for a specific asset
- **get_form**: Retrieve details for a specific form
- **get_job**: Retrieve details for a specific field job
- **get_me**: Check API connectivity and get user context
- **get_submission**: Retrieve details for a specific form submission
- **list_assets**: List all registered equipment assets
- **list_forms**: List all mobile forms
- **list_jobs**: List all field jobs/tasks
- **list_submissions**: List all data submissions for a specific form
- **list_users**: List all back-office and field users
- **update_job**: Modify an existing field job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Proforms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my account."

**🤖 AI Agent:**
> You have 2 active forms: 'Customer Feedback Survey' and 'Event Registration'.

---

**👤 You:**
> "Fetch the latest responses for form ID 8901."

**🤖 AI Agent:**
> Here are the last 3 submissions... User 'Alice' rated 5 stars, user 'Bob' requested support.

---

**👤 You:**
> "Summarize the feedback from 'Customer Feedback Survey'."

**🤖 AI Agent:**
> Out of 50 responses, 80% rated the service as 'Excellent'. The main complaint is regarding delivery times.


## Installation & Usage

To install and use the **Proforms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/proforms](https://vinkius.com/mcp/proforms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

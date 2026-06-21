# JobNimbus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jobnimbus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jobnimbus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jobnimbus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Manage contacts, jobs, and tasks via JobNimbus CRM API.

## Description
Empower your AI agents with JobNimbus's specialized CRM for contractors. This MCP server allows you to list and retrieve contacts and jobs, manage tasks and workflows, track payments, and view organization users directly through the JobNimbus API. Ideal for automating field service operations and project management.


## Available Tools
- **get_contact**: Returns addresses, phone numbers, email, and custom fields. Use this for deep intelligence on a customer before an interaction.

Retrieves details for a specific contact
- **get_job**: Returns project descriptions, associated contact IDs, and current workflow status. Use this to analyze project specifics or provide an update on a job.

Retrieves details for a specific job
- **list_boards**: Useful for navigating the account structure.

Lists all configured boards
- **list_contacts**: Returns names, contact types, and IDs. Use this to identify clients or start a search for a specific customer.

Lists all contacts in JobNimbus
- **list_jobs**: Includes job titles, status, and IDs. Essential for monitoring project flow and upcoming work.

Lists all jobs in JobNimbus
- **list_payments**: Essential for monitoring revenue and project billing status.

Lists all recent payments
- **list_products**: Useful for auditing available services and pricing items.

Lists all products and services
- **list_tasks**: Returns task descriptions, due dates, and IDs. Use this to help the user manage their daily workload or audit team activities.

Lists all tasks
- **list_users**: Useful for identifying sales reps or project managers.

Lists all users in the organization
- **list_workflows**: Useful for understanding the steps in the company's business processes.

Lists all configured workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JobNimbus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in JobNimbus."

**🤖 AI Agent:**
> I'll fetch the list of your contacts from JobNimbus for you.

---

**👤 You:**
> "Show me the latest jobs created."

**🤖 AI Agent:**
> I'll retrieve the most recent jobs from your JobNimbus account.

---

**👤 You:**
> "Check the status of my active tasks."

**🤖 AI Agent:**
> I'll look up your pending tasks and their current status in JobNimbus.


## Installation & Usage

To install and use the **JobNimbus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobnimbus](https://vinkius.com/mcp/jobnimbus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

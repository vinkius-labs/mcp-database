# CRM PipeRun MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crm-piperun)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crm-piperun-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crm-piperun-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage your sales pipeline and activities via PipeRun — track tasks, upload files, and organize deals directly from any AI agent.

## Description
Connect your **PipeRun CRM** account to any AI agent to streamline your sales operations through natural conversation.

### What you can do

- **Activity Management** — List, create, update, and delete tasks or appointments to keep your sales momentum.
- **File Handling** — Upload documents to deals, persons, or companies, and manage existing attachments effortlessly.
- **Activity Types** — Explore and categorize your interactions using specific activity types defined in your CRM.
- **Detailed Inspection** — Retrieve full metadata for specific activities or files to get the context you need.

### How it works

1. Subscribe to this server
2. Enter your PipeRun API Token
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — quickly update meeting notes and task statuses without leaving your workflow.
- **Sales Managers** — monitor team activities and file attachments across deals.
- **Operations Teams** — automate the organization of sales documents and activity logging.


## Available Tools
- **create_activity**: Create a new activity
- **delete_activity**: Delete an activity
- **delete_file**: Delete a file from PipeRun
- **get_activity**: Get details for a specific activity
- **get_activity_type**: Get details for a specific activity type
- **get_file**: Get details for a specific file
- **list_activities**: List activities (tasks and appointments)
- **list_activity_types**: List all activity types
- **list_files**: Supports pagination and filtering.

List files attached to deals, persons, or companies
- **update_activity**: Update an existing activity
- **upload_file**: Requires base64 encoded file content.

Upload a file to a deal, person, or company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CRM PipeRun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my activities for today from PipeRun."

**🤖 AI Agent:**
> I've retrieved your activities. You have 3 tasks scheduled: a 'Follow-up Call' with John Doe, a 'Contract Review' for Deal #445, and a 'Discovery Meeting' at 3 PM.

---

**👤 You:**
> "Upload this proposal to deal ID 12345."

**🤖 AI Agent:**
> The file 'Proposal_v1.pdf' has been successfully uploaded and attached to Deal 12345.

---

**👤 You:**
> "Create a new meeting activity for tomorrow morning."

**🤖 AI Agent:**
> I've created a new activity. Title: 'Client Meeting', Type: 'Meeting', Status: 'Open'. It is assigned to you for tomorrow.


## Installation & Usage

To install and use the **CRM PipeRun** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crm-piperun](https://vinkius.com/mcp/crm-piperun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

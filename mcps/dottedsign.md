# DottedSign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dottedsign)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dottedsign-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dottedsign-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

E-signature and document management with DottedSign.

## Description
The DottedSign MCP server empowers your AI agent to manage electronic signatures, retrieve document templates, and orchestrate signing tasks entirely from the conversational interface.


## Available Tools
- **cancel_task**: Cancel an active signing task
- **create_task_from_template**: Create a new signing task from a template
- **create_task**: Create a new signing task
- **delete_task**: Delete a signing task
- **get_audit_trail**: Get the audit trail for a specific task
- **get_me**: Get information about the current user/token
- **list_tasks**: List all signing tasks
- **list_templates**: List all available templates
- **list_users**: List all users in the account
- **list_webhooks**: List all configured webhooks
- **retrieve_task**: Get details of a specific signing task
- **update_task**: Update an existing signing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DottedSign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active document templates in DottedSign."

**🤖 AI Agent:**
> Retrieving your templates... You have 4 templates available. The most used one is 'Standard NDA'.

---

**👤 You:**
> "Check the status of signing task 'TASK_ID'."

**🤖 AI Agent:**
> Task 'TASK_ID' is currently 'Pending'. Only 1 out of 2 participants has signed.

---

**👤 You:**
> "Delete draft document 'DOC_ID'."

**🤖 AI Agent:**
> Draft document 'DOC_ID' has been successfully deleted from your workspace.


## Installation & Usage

To install and use the **DottedSign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dottedsign](https://vinkius.com/mcp/dottedsign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

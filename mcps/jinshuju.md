# Jinshuju / 金数据 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jinshuju)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jinshuju-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jinshuju-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Powerful online form and data collection platform — manage forms, entries, and webhooks via AI.

## Description
Empower your AI agent to orchestrate your data collection workflows with **Jinshuju** (金数据), the premier online form builder in China. By connecting Jinshuju to your agent, you transform complex form management, entry auditing, and lead collection into a natural conversation. Your agent can instantly list your forms, retrieve detailed submission data, create new entries programmatically, and even monitor webhook configurations without you ever needing to navigate the comprehensive web interface. Whether you are managing customer surveys or automated registration flows, your agent acts as a real-time data coordinator, keeping your information accurate and your responses organized.

### What you can do

- **Form Orchestration** — List all forms and retrieve detailed structures, field definitions, and settings.
- **Entry Management** — List, view, create, and update form submissions with full field support.
- **Data Auditing** — Retrieve real-time entry counts and monitor submission velocity for your forms.
- **Webhook Control** — Browse and monitor configured webhooks to ensure your data pipelines are healthy.
- **Workflow Integration** — Programmatically submit or modify entries to bridge your AI workflows with form data.

### How it works

1. Subscribe to this server
2. Enter your Jinshuju API Key and API Secret
3. Start managing your data collection through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Operations** — monitor lead generation and audit campaign forms through natural language queries.
- **Customer Research Teams** — retrieve survey responses and analyze qualitative data directly from your AI-powered workspace.
- **Operations Leads** — automate registration flows and monitor data entry consistency via a unified AI interface.
- **Jinshuju Power Users** — integrate your existing form workflows into your AI-driven daily routines.


## Available Tools
- **create_entry**: Submit a new entry
- **delete_entry**: Delete an entry
- **get_entry**: Get entry details
- **get_entry_count**: Get total entry count
- **get_form**: Get form details
- **get_form_fields**: Get form field definitions
- **list_entries**: List form entries
- **list_forms**: List all forms
- **list_webhooks**: List form webhooks
- **update_entry**: Update an entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jinshuju / 金数据** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my forms in Jinshuju."

**🤖 AI Agent:**
> I've retrieved your Jinshuju forms. You have 12 active forms, including 'Lead Registration V1' and 'Customer Feedback'. Would you like to see the entry count for any of them?

---

**👤 You:**
> "Show me the last 5 entries for form 'ABC-123'."

**🤖 AI Agent:**
> I've listed the last 5 entries for form ABC-123. They include submissions from 'Mario' and 'Renato'. Should I retrieve the full details for the most recent one?

---

**👤 You:**
> "Submit a new entry to form 'XYZ-789' with name 'John Doe' and email 'john@example.com'."

**🤖 AI Agent:**
> Done! I've programmatically submitted the new entry to form XYZ-789. The entry has been assigned serial number '8821'.


## Installation & Usage

To install and use the **Jinshuju / 金数据** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jinshuju](https://vinkius.com/mcp/jinshuju)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

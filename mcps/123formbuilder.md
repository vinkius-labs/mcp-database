# 123FormBuilder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/123formbuilder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/123formbuilder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/123formbuilder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build and manage online forms, collect submissions, and organize workspaces with AI-powered form automation for any workflow.

## Description
Connect your **123FormBuilder** account to any AI agent and simplify how you collect data, manage surveys, and analyze user submissions through natural conversation.

### What you can do
- **Form Management** — List all forms in your account, create new form containers, and retrieve detailed configuration metadata.
- **Submission Analysis** — List and query user data submitted to your forms, with pagination and detailed entry inspection.
- **Field Insights** — Query form structures to understand all input fields and data collection points.
- **Operational Oversight** — Monitor account status, list configured webhooks, and verify API connectivity.
- **Lifecycle Control** — Update form names or permanently remove unwanted forms and submissions via AI.

### How it works
1. Subscribe to this server
2. Enter your 123FormBuilder API Key (found in your account settings)
3. Start managing your data collection from Claude, Cursor, or any MCP client

### Who is it for?
- **Marketing & Research Teams** — quickly retrieve survey results and analyze submissions via simple AI commands.
- **Data Analysts** — monitor form performance and export entry data directly from the workspace.
- **Administrative Staff** — manage form organization and verify submission statuses via the AI assistant.


## Available Tools
- **create_new_form**: Add empty form
- **remove_form**: Delete form
- **remove_entry**: Delete submission
- **get_api_status**: Check connection
- **get_form_details**: Get form info
- **get_entry_details**: Read submission data
- **list_form_fields**: Get form structure
- **list_active_forms**: List account forms
- **list_form_entries**: Get submissions
- **list_form_webhooks**: Get event endpoints
- **test_formbuilder_auth**: Verify credentials
- **update_form_info**: Modify form name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **123FormBuilder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my 123FormBuilder account."

**🤖 AI Agent:**
> I've retrieved your forms. You have 3 active forms: 'Contact Us', 'Customer Feedback Survey', and 'Event Registration'. Which one would you like to see submissions for?

---

**👤 You:**
> "Show me the last 5 submissions for the 'Customer Feedback' form."

**🤖 AI Agent:**
> I've fetched the latest entries. There are 5 recent submissions. Most users mentioned high satisfaction, but one entry (ID: 5521) reported a layout issue. Shall I retrieve the details for that entry?

---

**👤 You:**
> "Update the name of form '10293' to 'Q4 Marketing Survey'."

**🤖 AI Agent:**
> Success! The form 10293 has been renamed to 'Q4 Marketing Survey'. This change is now reflected in your 123FormBuilder dashboard.


## Installation & Usage

To install and use the **123FormBuilder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/123formbuilder](https://vinkius.com/mcp/123formbuilder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

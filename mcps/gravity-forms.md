# Gravity Forms MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gravity-forms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gravity-forms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gravity-forms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your WordPress Gravity Forms — list forms, retrieve entries, and handle submissions directly via AI.

## Description
Connect your **Gravity Forms** REST API to any AI agent and take full control of your WordPress forms, entries, and submissions through natural conversation.

### What you can do

- **Form Orchestration** — List all forms on your site and inspect their fields and configuration structures natively
- **Entry Management** — Search and retrieve specific submissions, updating field values or trashing entries as needed
- **Automated Submissions** — Submit form data programmatically by passing field values, triggering all standard validation and notifications
- **Insights & Results** — Retrieve aggregate results and statistics for any form to analyze conversion rates and user data
- **Note Collaboration** — Read and add notes to specific entries to maintain internal team context within your helpdesk workflow
- **Feed & Notification Oversight** — Audit active feeds and notification settings to ensure your data is flowing correctly to external services

### How it works

1. Subscribe to this server
2. Enter your Site Base URL, Consumer Key, and Consumer Secret (generated in WordPress under Forms > Settings > REST API)
3. Start managing your lead generation and data collection from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Site Administrators** — audit form configurations and test submissions without manual browser interactions
- **Support Teams** — quickly look up customer form entries and add internal notes for better resolution tracking
- **Data Analysts** — extract form results and entry data for quick analysis and reporting through the chat interface


## Available Tools
- **create_entry_note**: Add a new note to a form entry
- **delete_entry**: Delete a form entry
- **get_entry**: Get detailed data for a specific form entry
- **get_form_results**: Get aggregate results and statistics for a specific form
- **get_form**: Get the structure and configuration of a specific form
- **get_notifications**: Get configured notifications for a specific form
- **list_entries**: Retrieve entries (submissions) for forms
- **list_entry_notes**: List all notes attached to a specific entry
- **list_feeds**: List all active feeds for a specific form
- **list_forms**: List all forms created in Gravity Forms
- **submit_form**: Submit a form programmatically
- **update_entry**: Update an existing form entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gravity Forms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my forms in Gravity Forms"

**🤖 AI Agent:**
> Retrieving your forms... I found 3 active forms: 'Contact Us' (ID: 1), 'Service Request' (ID: 2), and 'Customer Feedback' (ID: 3). Would you like to see the entries for the service request form?

---

**👤 You:**
> "Show me the entries for Form ID 1 from this week"

**🤖 AI Agent:**
> Fetching entries... I found 5 new submissions this week for the 'Contact Us' form. The latest is from John Doe (Entry #1042). Would you like to read the details of his message?

---

**👤 You:**
> "Add a note to entry #1042: 'Customer contacted support, refund processed'"

**🤖 AI Agent:**
> Adding note... Success! I've added the internal note to Entry #1042. It is now visible to the support team in your WordPress dashboard.


## Installation & Usage

To install and use the **Gravity Forms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gravity-forms](https://vinkius.com/mcp/gravity-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

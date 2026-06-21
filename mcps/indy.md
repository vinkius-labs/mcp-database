# Indy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/indy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/indy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your freelance business with proposals, contracts, time tracking, and invoicing that covers the entire client lifecycle.

## Description
Connect your **Indy** account to any AI agent and manage forms and records through natural conversation.

### What you can do

- **Form Management** — List all forms, inspect configurations, create new forms, and delete unused ones
- **Record Tracking** — Browse all form submissions, inspect individual records with full field data
- **Template Management** — List and inspect form templates for reusable designs
- **Group Organization** — Browse form groups for organized management
- **File Access** — List files attached to form submissions

### How it works

1. Subscribe to this server
2. Enter your Indy Access Token
3. Start managing forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — manage form submissions and track response data without the dashboard
- **Project Managers** — create intake forms, review submissions, and organize templates
- **Developers** — integrate form management into AI-driven workflows


## Available Tools
- **create_form**: Create a new form
- **create_webhook**: Create a new webhook
- **delete_form**: Delete a form
- **delete_webhook**: Delete a webhook
- **get_account_info**: Get account status
- **get_form**: Get form details
- **get_record**: Get submission details
- **get_user**: Get user details
- **list_forms**: List all forms
- **list_records**: List form submissions
- **list_users**: List connected users
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all forms and the latest submissions for the 'Customer Feedback' form."

**🤖 AI Agent:**
> Forms: 8 total. Active: 'Customer Feedback' (42 records), 'Job Application' (18 records), 'Event Registration' (65 records), 'Bug Report' (23 records), 4 others. Latest 'Customer Feedback' submissions: 1) Record #42 — Rating: 5/5, 'Great service, fast delivery'. 2) Record #41 — Rating: 3/5, 'Product quality good but shipping slow'. 3) Record #40 — Rating: 4/5, 'Would recommend'. Average rating: 4.2/5.

---

**👤 You:**
> "Create a new 'Event Registration' form and list available templates."

**🤖 AI Agent:**
> Form created! 'Event Registration' (form_089). Fields: Name, Email, Company, Ticket Type, Dietary Preferences. Status: Active. Shareable link ready. Templates: 6 available. 'Contact Form', 'Survey', 'Job Application', 'Feedback', 'Order Form', 'RSVP'. You now have 9 forms total.

---

**👤 You:**
> "Show all records for the bug report form and any attached files."

**🤖 AI Agent:**
> Bug Report form: 23 records. Priority breakdown: Critical (3), High (8), Medium (9), Low (3). Recent: Record #23 — 'Login button unresponsive on mobile' (Critical, with screenshot). Record #22 — 'Dashboard slow loading' (High). Files attached: 12 total across all records. Largest: screenshot_login_bug.png (2.1 MB, Record #23). Would you like to inspect a specific record?


## Installation & Usage

To install and use the **Indy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indy](https://vinkius.com/mcp/indy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

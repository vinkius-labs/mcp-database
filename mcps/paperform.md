# Paperform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/paperform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/paperform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage online forms and submissions via Paperform — list forms, track submissions, and configure webhooks directly from any AI agent.

## Description
Connect your **Paperform** account to any AI agent and take full control of your data collection workflows through natural conversation.

### What you can do

- **Form Oversight** — List all forms, retrieve detailed configurations, and manage your form library.
- **Submission Tracking** — List and retrieve detailed data for form submissions to analyze responses in real-time.
- **Webhook Management** — List and create webhooks for your forms to integrate with other services effortlessly.
- **Organizational Visibility** — List folders and custom domains to maintain a clear view of your account structure.
- **Metadata Auditing** — List all tags used across your forms to ensure consistent categorization.

### How it works

1. Subscribe to this server
2. Enter your Paperform Access Token (from Account Settings > API)
3. Start managing your forms directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Operations** — quickly check form submission counts or verify webhook configurations.
- **Customer Research** — retrieve and analyze form responses without leaving your chat interface.
- **Developers** — audit form metadata and integration settings during implementation.


## Available Tools
- **create_webhook**: Create a new webhook for a form
- **get_account_info**: Get authenticated account information
- **get_form**: Get details for a specific form
- **get_submission**: Get details for a specific submission
- **list_custom_domains**: List all custom domains configured
- **list_folders**: List all form folders
- **list_forms**: List all Paperform forms
- **list_submissions**: List submissions for a form
- **list_tags**: List all tags used in the account
- **list_webhooks**: List webhooks for a form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paperform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Paperform account."

**🤖 AI Agent:**
> I've retrieved 8 forms, including 'Contact Us', 'Product Feedback', and 'Event Registration'. Which one would you like to see submissions for?

---

**👤 You:**
> "Show me the last 5 submissions for the 'Event Registration' form."

**🤖 AI Agent:**
> I've fetched the latest 5 submissions. They include responses from 'John Doe', 'Jane Smith', and 3 others. Would you like the full details for any of these?

---

**👤 You:**
> "List all webhooks configured for form 'form_12345'."

**🤖 AI Agent:**
> There are 2 webhooks for this form: one pointing to Zapier and another to a custom endpoint (https://api.example.com/webhook).


## Installation & Usage

To install and use the **Paperform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperform](https://vinkius.com/mcp/paperform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

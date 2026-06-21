# Helpshift MCP Server

Automate mobile and web support via Helpshift — manage issues, FAQs, and user profiles directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/helpshift)

## Overview
**Category:** customer-support
**Tools Count:** 11

## Description
Connect your **Helpshift** platform to any AI agent and take full control of your customer support and user hub workflows through natural conversation.

### What you can do

- **Issue Oversight** — List all support issues, retrieve detailed metadata, and monitor audit logs for action history.
- **Response Management** — Add messages to existing issues and update statuses (Resolved, Rejected) directly from the chat.
- **Content Insights** — Browse your published FAQ articles and sections to ensure documentation is accurate.
- **User Hub Operations** — Perform bulk user profile updates and creation tasks using the User Hub v2 API.
- **Application Visibility** — List all registered apps in your Helpshift dashboard to ensure correct routing.
- **Operational Efficiency** — Track the progress of bulk identity tasks and monitor support volume in real-time.

### How it works

1. Subscribe to this server
2. Enter your Helpshift API Key and Domain
3. Start managing your support operations from Claude, Cursor, or any MCP-compatible client

No more manual exporting of issue logs. Your AI assistant acts as a dedicated Support Operations Lead or Mobile Support Specialist.

### Who is this for?

- **Support Managers** — instantly retrieve issue transcripts and audit logs to understand complex cases.
- **Mobile Product Teams** — monitor incoming bug reports and user feedback from within the development flow.
- **Customer Success Ops** — automate the management of large user profile batches and identity syncs.


## Available Tools
- **add_issue_message**: Pass the message details as a JSON string in "body_json".

Add a message to an existing issue
- **bulk_user_action**: Pass the actions array as a JSON string in "body_json".

Perform bulk profile operations (v2)
- **create_issue**: Pass the payload as a JSON string in "body_json" (requires app_id, title, body).

Create a new support issue
- **get_issue_audit_logs**: Retrieve the action history for a specific issue
- **get_bulk_task_status**: Check the status of a bulk profile operation
- **get_issue_details**: Get detailed information about a specific issue
- **list_registered_apps**: List all applications registered in your Helpshift dashboard
- **list_faqs**: List all published FAQ articles
- **list_issues**: Useful for monitoring support volume and identifying urgent cases.

List support issues/tickets in Helpshift
- **list_faq_sections**: List FAQ categories/sections
- **update_issue_status**: Update the status of an issue (e.g., Resolved, Rejected)


## Installation & Usage

To install and use the **Helpshift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpshift](https://vinkius.com/mcp/helpshift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

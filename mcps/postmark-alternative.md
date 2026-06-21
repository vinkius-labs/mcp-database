# Postmark MCP Server

Automate transactional email via Postmark — send emails, retrieve templates, inspect bounces, and manage your delivery analytics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-alternative)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect your **Postmark** server to any AI agent to fully orchestrate and analyze your transactional email pipeline.

### What you can do

- **Send Emails & Templates** — Send transactional emails directly from the agent using pre-configured Postmark Templates or Raw HTML.
- **Investigate Bounces** — Read the server bounce log to find out why specific recipients failed delivery (Hard Bounces, Blocks).
- **Template Management** — Fetch and review the raw body of your templates to ensure dynamic variables align flawlessly with code.
- **Outbound Analytics** — Review message stream stats, open rates, and general health metrics directly via chat.

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token
3. Gain complete control of your application's email notifications from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Software Engineers** — Trigger template dispatches from the terminal and review server logs to debug application email flows seamlessly.
- **Product Teams** — Monitor bounce rates and verify the visual layout of critical system emails without accessing the Postmark UI.
- **System Admins** — Quickly query delivery analytics and trace email endpoints for quick operational overviews.


## Available Tools
- **get_bounces_overview**: Get bounce overview analytics
- **get_server**: Get Postmark server details
- **get_template**: Get a specific Postmark template details
- **list_templates**: List templates in the server
- **get_outbound_overview**: Get outbound overview analytics
- **search_bounces**: You can filter by type, email, or message ID.

Search email bounces
- **search_outbound_messages**: You can filter by recipient, from email, or status.

Search outbound messages history
- **send_email**: Requires From, To, and either Subject/HtmlBody or Subject/TextBody.

Send a transactional email
- **send_email_with_template**: Send an email using a Postmark Template


## Installation & Usage

To install and use the **Postmark** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-alternative](https://vinkius.com/mcp/postmark-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

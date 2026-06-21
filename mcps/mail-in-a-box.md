# Mail-in-a-Box MCP Server

Manage mail users, aliases, and system health via the Mail-in-a-Box REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mail-in-a-box)

## Overview
**Category:** communication-messaging
**Tools Count:** 9

## Description
Connect your **Mail-in-a-Box** instance to any AI agent to automate your private email server management. This MCP server enables your agent to manage mailboxes, configure forwarding aliases, and monitor system health and diagnostics directly from natural language interfaces.

### What you can do

- **User Administration** — List all mail users, create new mailboxes, and update passwords programmatically
- **Alias Management** — Create, update, and remove email forwarding addresses and group aliases
- **System Monitoring** — Retrieve real-time health status, diagnostic checks, and configuration metadata for your server
- **Domain Oversight** — List all hosted mail domains and subdomains configured on your instance
- **Access Control** — Manage administrative privileges and account settings for your email users

### How it works

1. Subscribe to this server
2. Enter your Mail-in-a-Box Host, Admin Email, and Admin Password (or API Key)
3. Start managing your private email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **System Administrators** — Manage mailboxes and forwarding rules via simple natural language commands
- **DevOps Engineers** — Automate user onboarding and system health monitoring directly from your dev tools
- **Privacy-Conscious Teams** — Maintain your private communication infrastructure effortlessly through an AI-integrated interface


## Available Tools
- **create_mail_user**: Requires a full email address and a password.

Add a new mail user (mailbox)
- **list_mail_aliases**: List all mail aliases and forwarders
- **list_mail_domains**: List all mail domains hosted on the server
- **delete_mail_alias**: Remove a mail alias
- **delete_mail_user**: Remove a mail user
- **update_user_password**: Change the password for a mail user
- **get_system_status**: Check the status of the Mail-in-a-Box system
- **create_or_update_alias**: forwards_to should be a comma-separated list of emails.

Add or update a mail alias
- **list_mail_users**: List all mail users on the server


## Installation & Usage

To install and use the **Mail-in-a-Box** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mail-in-a-box](https://vinkius.com/mcp/mail-in-a-box)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

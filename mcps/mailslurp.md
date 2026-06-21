# MailSlurp MCP Server

Manage temporary inboxes and automate email testing via the MailSlurp REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailslurp)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your **MailSlurp** account to any AI agent to automate your email testing and asynchronous message management. This MCP server enables your agent to create virtual inboxes, send and receive emails, and handle complex automation scenarios using long-polling 'wait-for' methods directly from natural language interfaces.

### What you can do

- **Virtual Inbox Management** — Create random or custom email addresses and list all managed inboxes in your account
- **Email Automation** — Long-poll for the latest incoming email or wait until a specific email count is reached for testing suites
- **Message Retrieval** — List and inspect messages received by any virtual address, including full HTML and text bodies
- **Outbound Capability** — Send emails directly from any of your MailSlurp addresses programmatically
- **Infrastructure Maintenance** — Permanently delete individual messages or entire virtual inboxes via simple commands
- **Metadata Inspection** — Retrieve detailed technical headers and attachment metadata for any received email

### How it works

1. Subscribe to this server
2. Enter your MailSlurp API Key (x-api-key)
3. Start managing your virtual email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the verification of user registration flows and transactional alerts via natural language
- **Developers** — Quickly inspect incoming test emails and manage temporary addresses directly from your IDE
- **Product Teams** — Monitor and audit automated communication paths and email delivery results effortlessly


## Available Tools
- **create_random_inbox**: Create a new random email address
- **delete_specific_inbox**: Delete an inbox and its emails
- **list_inbox_emails**: List emails received by an inbox
- **get_email_details**: Get complete content for a specific email
- **list_all_inboxes**: List all MailSlurp inboxes
- **send_email_from_inbox**: Requires recipient and content.

Send an email using a MailSlurp address
- **wait_for_email_count**: Wait until an inbox has a certain number of emails
- **wait_for_latest_email**: Returns the latest one immediately if present.

Long-poll for the next incoming email


## Installation & Usage

To install and use the **MailSlurp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailslurp](https://vinkius.com/mcp/mailslurp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

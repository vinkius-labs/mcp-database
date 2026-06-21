# AfterLogic Aurora MCP Server

Email and webmail management — manage folders, messages, and accounts via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/afterlogic-aurora)

## Overview
**Category:** productivity
**Tools Count:** 5

## Description
Connect your **AfterLogic Aurora** account to your AI agent to unlock professional email and webmail orchestration. From managing complex mail folder structures to retrieving message lists and handling administrative account tasks, your agent handles your communication platform through natural conversation.

### What you can do

- **Mail Orchestration** — List and manage email folders and retrieve message lists for any account
- **Administrative Management** — Check if accounts exist and manage domains or users via the REST Admin API
- **Communication Flow** — Send and retrieve technical metadata for emails to support your communication workflows
- **Integration Support** — Access both the Web API for user-level tasks and the REST API for system-wide administration
- **Status Monitoring** — Quickly audit mail server availability and account statuses directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AfterLogic Aurora Base URL and Auth Credentials
3. Start managing your emails and mail accounts through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mail Administrators** — automate user provisioning and domain management effortlessly
- **IT Support Teams** — quickly check account statuses and folder structures to resolve inquiries
- **Developers** — integrate Aurora's mail capabilities into custom applications and workflows
- **Operations Leads** — monitor communication platform health and manage user access using simple commands


## Available Tools
- **list_folders**: Retrieve the internal email folder hierarchy for the authenticated AfterLogic user
- **list_messages**: Requires a folder path from list_folders.

Retrieve recent emails contained within a specified AfterLogic mail folder
- **send_email**: Compose and send an outbound email securely via the AfterLogic Web API
- **check_account_exists**: Requires Admin rights.

Verify if an email address is actively provisioned on the AfterLogic server
- **list_domains**: Requires Admin rights.

Retrieve all active custom domains mapped to the AfterLogic server instance


## Installation & Usage

To install and use the **AfterLogic Aurora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afterlogic-aurora](https://vinkius.com/mcp/afterlogic-aurora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# AfterLogic Aurora MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/afterlogic-aurora)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/afterlogic-aurora-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/afterlogic-aurora-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Email and webmail management — manage folders, messages, and accounts via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AfterLogic Aurora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mail folders for user 'admin@example.com'."

**🤖 AI Agent:**
> I've retrieved the folder list for admin@example.com. You have 5 standard folders: INBOX, Sent, Drafts, Spam, and Trash, along with 2 custom subfolders. Which folder would you like to open?

---

**👤 You:**
> "Check if the account 'user1@example.com' exists on the server."

**🤖 AI Agent:**
> I've checked the server records. The account 'user1@example.com' exists and is currently active. Would you like to see the quota usage for this account?

---

**👤 You:**
> "Show me the last 10 messages in the INBOX."

**🤖 AI Agent:**
> I've retrieved the latest 10 messages from your INBOX. They include 3 new inquiries, 2 system notifications, and several personal emails. Would you like the technical details for any specific message?


## Installation & Usage

To install and use the **AfterLogic Aurora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afterlogic-aurora](https://vinkius.com/mcp/afterlogic-aurora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

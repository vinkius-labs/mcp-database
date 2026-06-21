# Thinkific MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thinkific-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thinkific-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thinkific-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Manage Thinkific groups and webhooks — delete specific student groups and monitor site events directly from your AI agent.

## Description
Connect your **Thinkific** admin account to any AI agent to streamline your LMS management and event monitoring through natural conversation.

### What you can do

- **Group Administration** — Permanently delete specific student groups using their unique IDs to keep your dashboard organized.
- **Webhook Monitoring** — Retrieve a paginated list of all configured webhooks on your site to audit integrations and event triggers.
- **System Auditing** — Inspect webhook configurations including endpoints and limits to ensure your automated workflows are running correctly.

### How it works

1. Subscribe to this server
2. Enter your Thinkific API Key
3. Start managing your learning platform from Claude, Cursor, or any MCP-compatible client

No more digging through deep settings menus to find webhook URLs or clean up old groups. Your AI acts as a specialized LMS administrator.

### Who is this for?

- **Course Creators** — quickly clean up expired student groups without navigating the full admin UI.
- **LMS Developers** — audit and list active webhooks to debug integration flows directly from the terminal or code editor.
- **Operations Managers** — maintain site hygiene by managing organizational structures via simple commands.


## Available Tools
- **delete_group**: Delete a group in Thinkific
- **list_webhooks**: List Thinkific webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thinkific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all webhooks configured on my Thinkific site."

**🤖 AI Agent:**
> I've retrieved your webhooks. You have 3 active webhooks, including 'Order Created' pointing to your Zapier endpoint and 'Enrollment Completed'.

---

**👤 You:**
> "Delete the Thinkific group with ID 987654."

**🤖 AI Agent:**
> The group with ID 987654 has been successfully deleted from your Thinkific site.

---

**👤 You:**
> "Show me the first 5 webhooks on page 2."

**🤖 AI Agent:**
> Fetching page 2 with a limit of 5... I found 5 webhooks on this page. Would you like to see the details for any specific one?


## Installation & Usage

To install and use the **Thinkific** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thinkific-alternative](https://vinkius.com/mcp/thinkific-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

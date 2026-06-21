# Buttondown MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buttondown)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/buttondown-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/buttondown-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your newsletter via Buttondown — track subscribers, send emails, and monitor analytics directly from any AI agent.

## Description
Connect your **Buttondown** account to any AI agent and orchestrate your newsletter, subscriber management, and email campaigns through natural conversation.

### What you can do

- **Subscriber Oversight** — List all your subscribers and retrieve detailed profiles, including metadata and tags.
- **Email Management** — List all sent emails and drafts, and create new campaigns or drafts directly from your workspace.
- **Analytics Tracking** — Retrieve detailed analytics for specific emails, including open and click rates.
- **Segment Coordination** — Access and list your tags to ensure your audience is properly categorized.
- **Newsletter Access** — List all newsletters managed in your account and access your core profile settings.
- **Subscriber Growth** — Add new subscribers directly from your workspace with custom tags and metadata.

### How it works

1. Subscribe to this server
2. Enter your Buttondown API Key
3. Start managing your newsletter from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Content Creators** — quickly check subscriber counts or draft new updates without manual dashboard work.
- **Marketers** — retrieve email performance metrics and manage audience tags straight from their workflow tools.
- **Developers** — integrate newsletter subscription and campaign steps into their environment using natural language.


## Available Tools
- **create_email**: Create a new email or draft
- **create_subscriber**: Add a new subscriber to the newsletter
- **get_account_info**: Retrieve core account/profile settings
- **get_email_analytics**: Get analytics for a specific email
- **get_email**: Get details of a specific email
- **get_subscriber**: Get details of a specific subscriber
- **list_emails**: List all sent emails and drafts
- **list_newsletters**: List all newsletters in the account
- **list_subscribers**: List all newsletter subscribers
- **list_tags**: List all subscriber tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buttondown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my newsletter subscribers."

**🤖 AI Agent:**
> I've retrieved your subscribers. You have 150 active subscribers, including 'john.doe@example.com' and 'jane.smith@example.com'. Would you like to see details for a specific subscriber?

---

**👤 You:**
> "Show analytics for my last sent email."

**🤖 AI Agent:**
> Retrieving analytics... Your last email 'Weekly Updates #42' has a 45% open rate and a 12% click rate from 150 recipients.

---

**👤 You:**
> "Create a new draft with subject 'Hello World' and body 'This is a test'."

**🤖 AI Agent:**
> Draft 'Hello World' has been successfully created in your Buttondown account with ID email_99283.


## Installation & Usage

To install and use the **Buttondown** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buttondown](https://vinkius.com/mcp/buttondown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

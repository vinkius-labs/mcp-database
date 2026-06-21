# AWeber MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aweber-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aweber-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aweber-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate email marketing via AWeber — manage accounts, mailing lists, and subscribers directly from any AI agent.

## Description
Connect your **AWeber** account to any AI agent to streamline your email marketing workflows. Manage your subscribers and mailing lists through natural conversation.

### What you can do

- **Account Overview** — List all AWeber accounts associated with your access token.
- **List Management** — Retrieve and organize mailing lists for specific accounts.
- **Subscriber Operations** — List, add, and update subscribers within your mailing lists to keep your audience data current.
- **Data Synchronization** — Seamlessly pull subscriber details into your AI's context for better segmentation and analysis.

### How it works

1. Subscribe to this server
2. Enter your AWeber Access Token
3. Start managing your email campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — quickly check list growth and subscriber statuses without switching tabs.
- **Sales Teams** — add new leads to specific mailing lists directly from conversation or CRM workflows.
- **Growth Engineers** — automate subscriber updates and list querying within development environments.


## Available Tools
- **list_accounts**: List AWeber accounts
- **add_subscriber**: Add a new subscriber to a list
- **list_lists**: List mailing lists for an account
- **list_subscribers**: List subscribers in a mailing list
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWeber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AWeber accounts."

**🤖 AI Agent:**
> I've retrieved your accounts. You have access to 'Main Marketing' (ID: 123456). Would you like to see the mailing lists for this account?

---

**👤 You:**
> "Get the list of subscribers for account 12345 and list 67890."

**🤖 AI Agent:**
> Fetching subscribers for list 67890... I found 150 active subscribers. Would you like me to filter them or export the details?

---

**👤 You:**
> "Add 'john@example.com' with name 'John Doe' to list 67890 in account 12345."

**🤖 AI Agent:**
> Successfully added John Doe (john@example.com) to the mailing list. Their subscriber ID is 998877.


## Installation & Usage

To install and use the **AWeber** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aweber-alternative](https://vinkius.com/mcp/aweber-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Get a Newsletter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/get-a-newsletter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/get-a-newsletter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/get-a-newsletter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Send professional newsletters to your audience with an email platform that makes list management and campaign tracking simple.

## Description
Connect your **Get a Newsletter** account to any AI agent and take full control of your email marketing workflows through natural conversation.

### What you can do

- **Subscriber Management** — List, create, update, or remove email contacts directly from the cloud
- **Contact Inspection** — Fetch detailed metadata for specific subscribers and verify their status
- **List Organization** — View all active subscriber lists and create new audience segments
- **Campaign Tracking** — Retrieve sent and drafted email campaigns along with their details

### How it works

1. Subscribe to this server
2. Enter your Get a Newsletter API Token
3. Start managing your audience from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated marketing assistant, ready to sync leads or pull campaign data without opening the browser.

### Who is this for?

- **Marketers** — instantly retrieve campaign statuses or audience lists without leaving your workflow
- **Engineering Teams** — add or check subscribers straight from the code editor to verify integrations
- **Founders** — automate CRM cross-referencing by letting the agent query your active contacts


## Available Tools
- **create_contact**: Create a new contact (subscriber)
- **create_list**: Create a new subscriber list
- **delete_contact**: Delete a contact
- **get_campaign**: Get details of a specific campaign
- **get_contact**: Get details of a specific contact
- **get_list**: Get details of a specific list
- **list_campaigns**: List all campaigns
- **list_contacts**: List all contacts (subscribers)
- **list_lists**: List all subscriber lists
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Get a Newsletter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our email campaigns on Get a Newsletter."

**🤖 AI Agent:**
> I've fetched your campaigns. You have 'Q4 Product Launch' (sent) and 'Weekly Digest' (draft). Would you like to inspect any of them?

---

**👤 You:**
> "Add a new subscriber john.doe@example.com with the name John Doe."

**🤖 AI Agent:**
> Success! I have created the new contact John Doe (john.doe@example.com) in your Get a Newsletter audience.

---

**👤 You:**
> "Check if we have a subscriber list available and create a new one called 'Beta Testers'."

**🤖 AI Agent:**
> I found one existing list named 'Default Audience'. I have now created the new list 'Beta Testers' successfully.


## Installation & Usage

To install and use the **Get a Newsletter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/get-a-newsletter](https://vinkius.com/mcp/get-a-newsletter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

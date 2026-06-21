# Fidelizador MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fidelizador)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fidelizador-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fidelizador-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Build customer loyalty programs with points, rewards, and engagement campaigns that keep shoppers coming back.

## Description
Connect your **Fidelizador** account to any AI agent and take full control of your email marketing and automation workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage your email contacts programmatically, including creating, updating, and deleting profiles directly from your agent
- **Campaign Management** — Monitor your active and past email campaigns and retrieve detailed performance statistics and metadata programmatically
- **List Intelligence** — Create and manage mailing lists (segmentations) to maintain a structured and high-fidelity organization of your audience
- **Relational Integrity** — Access complete contact directories and retrieve granular details like phone numbers and custom data points
- **System Monitoring** — Check campaign statuses and manage subscriber lifecycles directly through your agent for instant marketing reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Fidelizador (Settings > Integrations)
3. Start managing your email marketing from Claude, Cursor, or any MCP client

No more manual subscriber management or complex campaign navigation in the dashboard. Your AI acts as your dedicated marketing and automation coordinator.

### Who is this for?

- **Digital Marketers** — instantly retrieve campaign results and update subscriber lists using natural language queries
- **CRM Managers** — maintain database hygiene by programmatically updating or deleting contacts without leaving your workspace
- **Sales Teams** — create new leads and manage mailing segments through simple AI commands


## Available Tools
- **create_contact**: Create a new contact
- **create_mailing_list**: Create a new mailing list
- **delete_contact**: Delete a contact
- **get_campaign**: Get campaign details
- **list_campaigns**: List email campaigns
- **list_contacts**: List contacts in Fidelizador
- **list_mailing_lists**: List mailing lists
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fidelizador** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns in Fidelizador."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active mailings, including 'Spring Promotion 2026' (ID: 101) and 'Product Newsletter'. Would you like the open rates for any of these?

---

**👤 You:**
> "Create a new contact 'John Doe' (john@example.com) in Fidelizador."

**🤖 AI Agent:**
> Contact created! John Doe has been successfully added to your Fidelizador database. Shall I add him to a specific mailing list now?

---

**👤 You:**
> "Show me the details for campaign ID '101'."

**🤖 AI Agent:**
> Fetching campaign 101... This 'Spring Promotion' had a 25% open rate and a 5% click-through rate. It was delivered to 1,500 recipients. Would you like a breakdown by list?


## Installation & Usage

To install and use the **Fidelizador** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fidelizador](https://vinkius.com/mcp/fidelizador)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

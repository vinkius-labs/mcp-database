# Zoho CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage leads, contacts, and deals on Zoho CRM — the AI-powered sales platform for growing teams.

## Description
Connect your **Zoho CRM** account to any AI agent and manage your entire sales lifecycle through natural conversation.

### What you can do

- **Lead Management** — List all CRM leads and retrieve comprehensive profile details to track potential customers through the sales funnel
- **Contact Discovery** — Browse your entire database of contacts and retrieve unique IDs for personalized engagement and follow-ups
- **Deal Monitoring** — Monitor active opportunities (deals) across your organization, retrieving pipeline stages and transaction values
- **Account Auditing** — List company accounts and retrieve metadata to understand organizational relationships within your CRM
- **Product Access** — Browse your product catalog directly from your agent to verify availability and pricing details
- **Activity Tracking** — List assigned tasks and logged calls to stay on top of your team's daily sales activities and productivity
- **Deep Discovery** — Quickly find unique lead, contact, deal, and account IDs required for automated CRM workflows

### How it works

1. Subscribe to this server
2. Enter your Zoho Access Token and API Domain (e.g., accounts.zoho.com)
3. Start managing your sales pipeline through Claude, Cursor, or any MCP-compatible client

No more manual filtering through complex CRM views to find a lead's phone number. Your AI agent becomes your sales operations assistant.

### Who is this for?

- **Sales Professionals** — quickly lookup lead details and monitor active deals through simple chat commands
- **Account Managers** — browse company accounts and contact profiles without manual navigation
- **Marketing Teams** — verify lead ingestion and monitor product catalog details for campaign alignment
- **Operations Teams** — audit tasks and call logs to ensure CRM data integrity and team productivity


## Available Tools
- **list_accounts**: List all accounts
- **list_calls**: List all calls
- **list_contacts**: List all contacts
- **list_deals**: List all deals
- **get_contact**: Get contact details
- **get_deal**: Get deal details
- **get_lead**: Get lead details
- **list_leads**: Useful for lead management and tracking.

List all CRM leads
- **list_products**: List all products
- **list_tasks**: List all tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 leads in my Zoho CRM account."

**🤖 AI Agent:**
> I found your 5 most recent leads: 1. John Doe (Acme Corp), 2. Jane Smith (Global Tech), 3. Robert Brown (Stark Industries), and 2 others. Which one would you like to see the contact details for?

---

**👤 You:**
> "What is the current status of the deal with ID '12345678'?"

**🤖 AI Agent:**
> Deal 'Enterprise Expansion' (ID: 12345678): Stage: Negotiation/Review, Value: $45,000.00, Expected Closing: 2026-04-15. Owner: Alice Johnson. Would you like me to check for any recent call logs related to this deal?

---

**👤 You:**
> "List all tasks assigned to me in Zoho CRM."

**🤖 AI Agent:**
> I found 4 active tasks assigned to you: 1. 'Follow up with John Doe', 2. 'Draft proposal for Global Tech', 3. 'Verify billing for Stark Industries', and 4. 'Update product catalog'. Which one would you like to update?


## Installation & Usage

To install and use the **Zoho CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm](https://vinkius.com/mcp/zoho-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

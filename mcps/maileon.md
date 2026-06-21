# Maileon MCP Server

Manage email marketing contacts, mailings, and reporting via the Maileon REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/maileon)

## Overview
**Category:** marketing-automation
**Tools Count:** 9

## Description
Connect your **Maileon** account to any AI agent to automate your professional email marketing and audience management. This MCP server enables your agent to manage subscribers, control mailing lifecycles, and retrieve detailed performance statistics directly from natural language interfaces.

### What you can do

- **Contact Management** — List all subscribers, retrieve complete profiles by email, and manage opt-ins and opt-outs
- **Mailing Control** — Monitor your email campaigns (mailings), retrieve metadata, and trigger official dispatches when ready
- **Real-time Reporting** — Retrieve KPIs and statistics for individual mailings, including opens, clicks, and bounces
- **Audience Hygiene** — Monitor unsubscription events and permanently remove contacts to maintain list quality
- **Data Ingestion** — Create and update subscriber records programmatically to sync with your external CRMs

### How it works

1. Subscribe to this server
2. Enter your Maileon REST API Key
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **CRM Managers** — Monitor campaign statuses and manage subscriber lists via simple natural language commands
- **Marketing Operations** — Quickly check mailing performance and manage contact updates without opening the portal
- **Developers** — Integrate Maileon's advanced mailing logic and reporting into your custom internal tools


## Available Tools
- **list_account_contacts**: Use optional params for filtering.

List all contacts in the Maileon account
- **create_new_contact**: Can trigger a Double Opt-In process if configured.

Add or update a contact in the database
- **delete_account_contact**: Remove a contact from the account
- **dispatch_email_mailing**: The mailing must be in a ready state.

Trigger the dispatch of a mailing
- **get_contact_by_email**: Get details for a specific contact
- **get_mailing_details**: Get details for a specific mailing
- **get_mailing_statistics**: Get performance statistics for a mailing
- **list_email_mailings**: Use optional params to filter by state (e.g., "state=draft").

List all mailings (campaigns)
- **list_unsubscription_events**: List recent unsubscription events


## Installation & Usage

To install and use the **Maileon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maileon](https://vinkius.com/mcp/maileon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

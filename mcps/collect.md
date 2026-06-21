# Collect MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/collect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/collect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/collect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Enable your AI agent to manage data collection campaigns, send requests, and track submissions via the Collect API.

## Description
Connect your AI to **Collect**, the secure platform for gathering information and documents from clients.

### What you can do

- **Campaign Management** — List active data collection campaigns and check their completion status.
- **Request Sending** — Send new data requests to clients by email for KYC, onboarding, or compliance workflows.
- **Status Tracking** — Check the status of individual requests, view messages, and monitor completion.

### How it works

1. Add the Collect integration to your AI toolset.
2. Provide your API Key (from Settings > Integrations > API).
3. Manage your data collection workflows via natural language.

### Who is this for?

- **Compliance Teams** — Send and track KYC requests without switching to the Collect dashboard.
- **Accounting Firms** — Manage document collection campaigns for multiple clients from chat.
- **HR Teams** — Track onboarding document submissions and send reminders.


## Available Tools
- **send_message**: Send a message to a recipient regarding a specific request
- **create_request**: Send a new data collection request to a recipient
- **get_campaign**: Retrieve detailed information about a specific campaign
- **get_element_details**: Retrieve details of a specific element (field/block) in a request
- **get_request**: Retrieve details of a specific data request
- **get_team_info**: Retrieve information about your team in Collect
- **get_user_info**: Retrieve information about the currently authenticated user
- **list_campaigns**: Retrieve a list of all data collection campaigns in Collect
- **list_messages**: Retrieve a list of messages sent through Collect
- **list_requests**: Retrieve all data requests for a specific campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active data collection campaigns."

**🤖 AI Agent:**
> You have 3 active campaigns:
1. 'KYC Process' — 12/20 requests completed (60%)
2. 'Tax Documents 2025' — 45/50 requests completed (90%)
3. 'New Client Onboarding' — 3/8 requests completed (37%)
Want to send reminders for pending requests?

---

**👤 You:**
> "Send a data request to 'John Doe' (john@example.com) for the 'KYC Process' campaign."

**🤖 AI Agent:**
> Request sent to John Doe (john@example.com) for campaign 'KYC Process'. Request ID: req-7x2k. Status: pending. The client will receive an email with the secure link.

---

**👤 You:**
> "Send an automatic reminder to all clients with missing documents in the 'Tax 2025' campaign."

**🤖 AI Agent:**
> Done. Reminders were successfully sent to 5 pending clients in the 'Tax Documents 2025' campaign. The clients have been re-notified.


## Installation & Usage

To install and use the **Collect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/collect](https://vinkius.com/mcp/collect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

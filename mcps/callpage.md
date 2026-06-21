# CallPage MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callpage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/callpage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/callpage-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage callbacks and leads via CallPage — track calls, manage widgets, and coordinate with your sales team directly from any AI agent.

## Description
Connect your **CallPage** account to any AI agent and orchestrate your lead generation, callback management, and team productivity through natural conversation.

### What you can do

- **Call Oversight** — List all callback calls and retrieve detailed metadata, including recording URLs and durations.
- **Lead Management** — List all captured leads from your widgets and retrieve detailed profiles, including contact info and intent.
- **Widget Control** — List all your CallPage widgets and retrieve their specific configuration and performance settings.
- **Team Coordination** — Access your directory of managers and departments to ensure incoming leads are properly routed.
- **Sms Templates** — List available SMS templates used for automated follow-ups.
- **Account Insights** — Retrieve core manager and account information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your CallPage External API Key
3. Start managing your lead pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & SDR Teams** — quickly check new leads or listen to call recordings without manual dashboard logins.
- **Marketing Managers** — monitor widget performance and lead quality straight from their workflow tools.
- **Customer Success** — retrieve department info and manager settings using natural language.


## Available Tools
- **get_account_info**: Retrieve core manager/account info
- **get_call_details**: Get details of a specific call
- **get_lead_details**: Get details of a specific lead
- **get_widget_settings**: Get settings for a specific widget
- **list_calls**: List all callback calls and their recordings
- **list_departments**: List company departments
- **list_leads**: List captured leads from widgets
- **list_managers**: List team managers
- **list_sms_templates**: List available SMS templates
- **list_widgets**: List all CallPage widgets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallPage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my leads from today in CallPage."

**🤖 AI Agent:**
> I've retrieved your leads. You have 5 new leads today, including 'John Doe' (+1234567890) and 'Sarah Smith' (intent: inquiry).

---

**👤 You:**
> "Show the last 3 call recordings."

**🤖 AI Agent:**
> Retrieving recent calls... I found 3 recordings: Call #101 (2m 30s), Call #105 (1m 15s), and Call #109 (4m 45s). You can listen to them here: [Links].

---

**👤 You:**
> "What are the settings for widget 'Main Website'?"

**🤖 AI Agent:**
> Widget 'Main Website' (ID: wid_123) is currently active. It has 'Delayed Callback' enabled (28 seconds) and is assigned to the 'Sales' department.


## Installation & Usage

To install and use the **CallPage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callpage](https://vinkius.com/mcp/callpage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

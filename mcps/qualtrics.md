# Qualtrics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qualtrics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qualtrics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qualtrics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Automate survey management and data collection via Qualtrics — list surveys, manage distributions, and export responses directly from any AI agent.

## Description
Connect your **Qualtrics** account to any AI agent and take full control of your Experience Management (XM) workflows through natural conversation.

### What you can do

- **Survey Lifecycle** — List all available surveys, fetch detailed metadata, and create or update survey structures programmatically.
- **Response Data Extraction** — Trigger response exports, monitor their progress, and retrieve the final data files (CSV/JSON) for deep analysis.
- **Distribution Management** — List and create survey distributions to reach your audience across different channels.
- **XM Directory & Contacts** — Manage your contact lists by listing directory members or creating/updating contact information directly.
- **Event Subscriptions** — List and create event subscriptions to build reactive workflows based on survey activities.

### How it works

1. Subscribe to this server
2. Enter your Qualtrics API Token and Datacenter ID
3. Start managing your research projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — instantly check survey statuses and export response data without navigating the Qualtrics UI
- **Customer Success Leads** — manage contact directories and distributions to automate feedback loops
- **Data Analysts** — pull raw survey data directly into your analysis environment via AI-driven export commands


## Available Tools
- **create_contact**: Create a new contact in an XM Directory
- **create_distribution**: Create a new distribution for a survey
- **create_event_subscription**: Create a webhook event subscription
- **create_response_export**: Start a response export for a survey
- **create_survey**: Create a new survey
- **get_distribution**: Get details for a specific distribution
- **get_export_file**: Get the exported file for a survey response export
- **get_export_progress**: Check the progress of a response export
- **get_survey**: Get details for a specific survey
- **list_directory_contacts**: List contacts in an XM Directory
- **list_distributions**: List distributions for a survey
- **list_event_subscriptions**: List all webhook event subscriptions
- **list_surveys**: List all Qualtrics surveys
- **update_contact**: Update an existing contact in an XM Directory
- **update_survey**: Update an existing survey


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qualtrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Qualtrics surveys."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 3 active surveys: 'Customer Satisfaction 2024' (ID: SV_123), 'Employee Engagement' (ID: SV_456), and 'Product Feedback' (ID: SV_789).

---

**👤 You:**
> "Create a new survey named 'Market Research Q3' in English."

**🤖 AI Agent:**
> The survey 'Market Research Q3' has been successfully created with ID: SV_98765. You can now start adding questions or setting up distributions.

---

**👤 You:**
> "Export the responses for survey SV_12345 in CSV format."

**🤖 AI Agent:**
> I've initiated the export for survey SV_12345. The Export ID is ES_abc123. I will monitor the progress for you.


## Installation & Usage

To install and use the **Qualtrics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qualtrics](https://vinkius.com/mcp/qualtrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

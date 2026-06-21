# Cognito Forms MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cognito-forms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cognito-forms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cognito-forms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build smart online forms with conditional logic, calculations, and payment collection that adapt to every response.

## Description
Connect your **Cognito Forms** account to any AI agent and take full control of your automated data collection and form management workflows through natural conversation.

### What you can do

- **Form Orchestration** — List and manage your active and archived online forms programmatically, including retrieving detailed metadata and entry counts
- **Entry Intelligence** — Access form submissions in real-time, including status tracking and historical metadata to coordinate deep data analysis
- **Schema Discovery** — Access the full JSON schema for any form to understand internal field structures and validation rules programmatically
- **Direct Data Capture** — Programmatically create new form entries from your AI agent to accelerate your data ingestion and lead capture cycles
- **Operational Visibility** — Retrieve specific entry details and monitor form volume directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from Cognito Forms settings (Organization Settings > API Tokens)
3. Start managing your forms and data entries from Claude, Cursor, or any MCP client

No more manual exporting of entries or searching through form folders in the portal. Your AI acts as your dedicated data coordinator and form operations analyst.

### Who is this for?

- **Operations Managers** — instantly retrieve form submission summaries and check entry statuses using natural language commands
- **Data Analysts** — automate the retrieval of structured form data for reporting and cross-platform analysis without leaving your workspace
- **Developers** — integrate real-time form intelligence and entry management into custom workflows through simple AI queries


## Available Tools
- **check_cognito_status**: Verify connectivity
- **create_entry**: Create an entry
- **delete_entry**: Delete an entry
- **get_entry**: Get entry details
- **get_form_fields**: Get form fields
- **get_form**: Get form schema
- **list_entries**: List entries
- **list_forms**: List forms
- **list_organizations**: List organizations
- **list_templates**: List templates
- **search_entries**: Search entries
- **update_entry**: Update an entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cognito Forms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my Cognito account."

**🤖 AI Agent:**
> I've retrieved your forms. You currently have 3 active projects: 'Customer Support' (ID: support-v1), 'Sales Intake', and 'Feedback Survey'. Which one would you like to see the entries for?

---

**👤 You:**
> "Show the last 5 entries for the 'Sales Intake' form."

**🤖 AI Agent:**
> Fetching entries... I found 5 recent submissions for 'Sales Intake'. Highlights include a new lead from @user1 and a pricing inquiry. Would you like the detailed field values for the latest lead?

---

**👤 You:**
> "Get the JSON schema for form ID 'feedback-survey'."

**🤖 AI Agent:**
> I've retrieved the schema for 'feedback-survey'. The form expects 4 main fields: 'Rating' (Numeric), 'Comments' (Long Text), 'Email', and 'SubmitDate'. I'm ready to create a new entry for you.


## Installation & Usage

To install and use the **Cognito Forms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cognito-forms](https://vinkius.com/mcp/cognito-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Formsite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formsite)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/formsite-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/formsite-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage forms, retrieve results, and automate data collection via AI agents with Formsite.

## Description
Connect your **Formsite** account to any AI agent to automate your form results retrieval and data management through the Model Context Protocol (MCP). Formsite is a professional form builder that enables organizations to create sophisticated forms and surveys. This MCP server allows you to list your forms, fetch real-time results, and manage webhooks directly through natural conversation.

### What you can do

- **Results Retrieval** — List and fetch form submissions/results instantly, including detailed answers and timestamps.
- **Form Oversight** — Access and list all forms in your account to maintain full visibility of your active data collectors.
- **Field Inspection** — Retrieve the fields and items defined within your forms to understand the structure of your data.
- **Webhook Automation** — Create and manage webhooks to receive real-time notifications when new results are completed.
- **Reporting Insights** — List and retrieve reports defined for your forms to get high-level snapshots of your data.
- **Multi-Server Support** — Seamlessly connect to your specific Formsite server environment (e.g., fs18).

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Formsite Server, User Directory, and Access Token (found in Settings > Integrations > Formsite API)
3. Start managing your form data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly pull form results for analysis or list report metadata without leaving your primary agent.
- **Operations Teams** — automate the monitoring of new form submissions and webhook configurations.
- **Customer Feedback Managers** — manage sophisticated surveys and retrieve user sentiment via simple AI commands.


## Available Tools
- **create_webhook**: Create a new webhook
- **delete_webhook**: Remove a webhook
- **get_form_details**: Get form metadata
- **get_form_reports**: Get form reports
- **list_form_items**: List form fields
- **list_forms**: List all forms
- **list_results**: List form results
- **list_webhooks**: List form webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formsite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Formsite account and their directory names."

**🤖 AI Agent:**
> Retrieving forms... I found 5 forms, including 'Annual Survey' (dir: survey_2023) and 'Contact Form' (dir: contact_us). Which one would you like to check results for?

---

**👤 You:**
> "Show me the 10 most recent results for form 'survey_2023'."

**🤖 AI Agent:**
> Fetching results... For survey_2023, I found 10 recent submissions. Key feedback includes requests for 'Faster shipping' and 'More color options'.

---

**👤 You:**
> "What fields are defined in my 'Contact' form (dir: contact_us)?"

**🤖 AI Agent:**
> Inspecting form items... The 'Contact Form' includes fields for 'Name', 'Email Address', 'Subject', and 'Message (Paragraph Text)'.


## Installation & Usage

To install and use the **Formsite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formsite](https://vinkius.com/mcp/formsite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

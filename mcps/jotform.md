# JotForm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jotform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jotform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jotform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage forms, submissions, and reports via JotForm API.

## Description
Empower your AI agents with JotForm's powerful online form builder. This MCP server allows you to list and retrieve forms, track submissions, manage reports and folders, and view account usage directly through the JotForm API. Ideal for automating data collection and form management workflows.


## Available Tools
- **get_account**: Use to verify account status or identity.

Retrieves details about your JotForm account
- **get_form**: Returns form properties and the list of questions/fields. Essential for understanding what data a form collects or before analyzing its submissions.

Retrieves details/questions for a specific form
- **get_form_submissions**: Returns individual response details. Use this when the user wants to analyze the results of a particular survey or contact form.

Retrieves all submissions for a specific form
- **get_usage**: Use this to inform the user if they are approaching their plan capacity.

Retrieves account usage limits and current status
- **list_folders**: Useful for navigating large accounts with many forms organized by department or project.

Lists folders used to organize forms
- **list_forms**: Returns form titles, IDs, and response counts. Use this as the main starting point to browse available forms or locate a specific form ID.

Lists all forms in your JotForm account
- **list_history**: Use this for auditing account usage and recent management actions.

Lists account activity history
- **list_reports**: Useful for identifying pre-aggregated data views.

Lists all generated reports
- **list_submissions**: Use this to monitor general submission activity or identify recent entries across multiple forms.

Lists all submissions across all forms
- **list_webhooks**: Useful for debugging automation flows.

Lists configured webhooks for a specific form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JotForm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my JotForm account."

**🤖 AI Agent:**
> I'll fetch the list of available forms from your JotForm account.

---

**👤 You:**
> "Show me the submissions for form ID '123'."

**🤖 AI Agent:**
> I'll retrieve the submissions for that specific form from JotForm.

---

**👤 You:**
> "Check my account usage limits."

**🤖 AI Agent:**
> I'll look up the usage statistics and limits for your JotForm account.


## Installation & Usage

To install and use the **JotForm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jotform](https://vinkius.com/mcp/jotform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

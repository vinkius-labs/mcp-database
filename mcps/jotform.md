# JotForm MCP Server

Manage forms, submissions, and reports via JotForm API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jotform)

## Overview
**Category:** productivity
**Tools Count:** 10

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


## Installation & Usage

To install and use the **JotForm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jotform](https://vinkius.com/mcp/jotform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

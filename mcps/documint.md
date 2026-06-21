# Documint MCP Server

Equip your AI agent to automate document generation, manage templates, and track output files via the Documint API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/documint)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Documint**, the versatile document generation and automation platform, directly into your AI workflow. Manage your dynamic document templates, generate professional PDF files from JSON data, and track your generation history using natural language.

### What you can do

- **Template Oversight** — List and retrieve detailed configuration and variable schemas for all your document templates.
- **Document Generation** — Trigger the Documint engine to create new files instantly using provided data variables.
- **Generation Tracking** — Monitor the status of your document generations and access secure download URLs.
- **Variable Intelligence** — Identify exactly which data keys are required to populate specific templates accurately.

### How it works

1. Connect the Documint integration to your AI assistant.
2. Authorize using your Documint API Key (found in your account settings).
3. Orchestrate your document automation and reporting through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly generate invoices or proposals from CRM data on the go.
- **Accountants** — Monitor document generation status and access output files for billing via chat.
- **Developers** — Audit template variables and test document generation logic instantly.


## Available Tools
- **create_new_generation**: Generate a new document using a specific template and data object
- **get_documint_account_metadata**: Retrieve metadata and usage limits for your Documint account
- **get_generation_details**: Get the current status and download URL for a specific generated document
- **get_template_variable_audit**: Identify exactly which variables are required to populate a template
- **get_template_configuration**: Get detailed information and field schema for a specific template
- **list_documint_generations**: List all documents that have been generated in Documint
- **list_failed_doc_generations**: Identify document generations that failed due to errors (mock logic)
- **list_latest_doc_generations**: Identify the most recently generated documents
- **list_documint_templates**: List all available document templates in your Documint account
- **search_documint_templates**: Search for a document template using a name keyword


## Installation & Usage

To install and use the **Documint** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/documint](https://vinkius.com/mcp/documint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

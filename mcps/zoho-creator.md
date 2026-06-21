# Zoho Creator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-creator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-creator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-creator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Low-code platform to build applications and manage records with AI using Creator API v2.1.

## Description
Connect your **Zoho Creator** account to any AI agent to automate your business application workflows through natural conversation. Perform CRUD operations, manage structural metadata, and navigate your low-code ecosystem with ease.

### What you can do

- **Record Management** — Perform full CRUD operations on records directly through forms and reports in your applications.
- **Structural Metadata** — Retrieve detailed metadata for your applications, including form and report definitions and field types.
- **App Navigation** — List all accessible applications and workspaces to stay organized across your Creator environment.
- **Workflow Control** — Automate data entry and updates with support for skipping workflow triggers when necessary (skip_workflow).
- **Structural Sync** — Maintain architectural integrity by programmatically accessing structural definitions of your low-code apps.

### How it works

1. Subscribe to this server
2. Enter your Zoho Creator OAuth Access Token (Zoho-oauthtoken)
3. Provide your Account Owner name and select your Data Center URL
4. Start managing your low-code apps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Analysts** — automate data management and reporting workflows without manual entry.
- **Low-code Developers** — programmatically interact with Creator apps and manage structural metadata.
- **IT Teams** — streamline application management and data synchronization across the Zoho ecosystem.


## Available Tools
- **add_record**: Create new record
- **delete_record**: Remove record
- **get_api_status**: Get connection status
- **get_form_fields**: Get field definitions
- **get_app_metadata**: Get app structural info
- **get_record_details**: Get record by ID
- **get_report_records**: Fetch records from report
- **list_applications**: List Zoho Creator apps
- **list_app_forms**: List application forms
- **list_app_reports**: List application reports
- **list_workspaces**: List creator workspaces
- **update_record**: Modify existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the metadata and form fields for the 'Employee Directory' application so I can see what data is collected."

**🤖 AI Agent:**
> I've fetched the metadata for 'Employee Directory'. The main form 'Add_Employee' contains 6 fields: Full_Name, Email, Department, Joining_Date, Salary, and Manager_ID. Would you like me to add a new record to it?

---

**👤 You:**
> "Add a new record to the 'Inventory Manager' app under the 'Products' form with Name 'Ergonomic Chair' and Price '199.99'."

**🤖 AI Agent:**
> The record for 'Ergonomic Chair' has been successfully added to the 'Products' form in the 'Inventory Manager' application. The new record ID is 38920188492001.

---

**👤 You:**
> "Fetch the latest records from the 'Sales Tracker' report where the status is 'Pending Approval'."

**🤖 AI Agent:**
> I've retrieved the records from the 'Sales Tracker' report. There are currently 4 sales records with the status 'Pending Approval'. The highest value deal is 'Acme Corp Contract' at $45,000.


## Installation & Usage

To install and use the **Zoho Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-creator](https://vinkius.com/mcp/zoho-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

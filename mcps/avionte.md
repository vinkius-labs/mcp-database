# Avionte MCP Server

Manage staffing and recruiting workflows via Avionte — query talent profiles, work history, company details, and department data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/avionte)

## Overview
**Category:** human-resources
**Tools Count:** 16

## Description
Connect your **Avionte** staffing platform to any AI agent and streamline your recruitment and talent management workflows through natural conversation.

### What you can do

- **Talent Management** — Retrieve comprehensive talent profiles, including work history, education records, and current nomination stages.
- **Company & Department Insights** — Fetch detailed information about companies, specific departments, and their physical addresses.
- **Payroll & Banking** — Securely access talent direct deposit account information and banking details for administrative tasks.
- **Workflow Tracking** — Monitor talent tags, available statuses, and company-specific purchase orders (POs) to keep your staffing operations organized.
- **Data Categorization** — List and manage tags for both talent and companies to ensure precise filtering and reporting.

### How it works

1. Subscribe to this server
2. Enter your Avionte API Key, Client ID, Client Secret, and Tenant ID
3. Start managing your staffing pipeline from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated recruiting coordinator, providing instant access to candidate data and organizational structures without switching between multiple software modules.

### Who is this for?

- **Recruiters & Sourcers** — quickly pull candidate backgrounds and check nomination stages during the screening process.
- **HR Operations** — verify banking details and education history for onboarding without manual data entry.
- **Account Managers** — retrieve company tags and department structures to better serve client staffing needs.


## Available Tools
- **get_all_talent_tags**: Get all tags associated with a talent
- **get_available_talent_statuses**: List all available talent statuses
- **get_company_po_by_po_id**: Retrieve a specific purchase order
- **get_company_restrictions**: Get talent restrictions for a company
- **get_company_tags**: Get tags for a company
- **get_company**: Retrieve company details
- **get_department_address**: Get a specific department address
- **get_department**: Retrieve department details
- **get_job**: Retrieve job details
- **get_multiple_pipeline_by_pipeline_ids**: Get details for multiple job pipelines
- **get_talent_direct_deposit_accounts**: Get direct deposit accounts for a talent
- **get_talent_education_history**: Retrieve education history for a talent
- **get_talent_stage**: Get details about a talent nomination stage
- **get_talent**: Provide talentId or other query parameters as needed.

Retrieve details for a specific talent
- **get_talent_work_history**: Retrieve work history for a talent
- **get_web_applications_for_talent**: List jobs a talent has applied for


## Installation & Usage

To install and use the **Avionte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avionte](https://vinkius.com/mcp/avionte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

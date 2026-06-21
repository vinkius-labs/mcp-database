# Zoho CRM Analytics MCP Server

Access custom views, organization info, module metadata, fields, and pipeline analysis in Zoho CRM.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-analytics)

## Overview
**Category:** data-analytics
**Tools Count:** 5

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools
- **zoho_module_fields**: Returns field name, display label, data type (text/number/date/picklist/lookup), whether it is required, read-only, and formula-based. Essential for understanding the data model before creating or updating records. Use when the user asks "what fields are on Contacts?" or needs to know valid field names for API operations.

Get all fields (properties) configured on a Zoho CRM module with data types, validation rules, and edit permissions
- **zoho_org_info**: Returns company name, Zoho CRM edition (Free/Standard/Professional/Enterprise/Ultimate), default timezone, currency, and admin contact. Use when the user needs account-level information, subscription details, or org configuration.

Get Zoho CRM organization details — company name, subscription edition, timezone, currency, and license information
- **zoho_custom_views**: Returns view name, system name, category (shared/personal), and whether it is the default. Custom views are saved filters that define how records appear in the module list view (e.g., "All Open Deals", "My Contacts", "Unread Leads"). Use when the user asks about available filters, saved views, or list configurations.

List saved custom views/filters for a Zoho CRM module — predefined list views like "My Open Deals" or "All Leads"
- **zoho_list_modules**: Returns module name, plural label, API name, whether the module supports API access, and visibility status. Modules include: Leads, Contacts, Accounts, Deals, Tasks, Events, Calls, Notes, Products, Quotes, Sales_Orders, Invoices, Purchase_Orders, and custom modules. Use to discover the data model or verify which modules are available.

List all available CRM modules in Zoho with their names, API support status, and whether they are visible
- **zoho_list_pipelines**: For deals: shows sales pipeline stages with associated win probability percentages (e.g., Qualification=10%, Proposal=75%, Closed Won=100%). Returns pipeline name, stage names, stage IDs, and probabilities. Use to understand the sales process, find stage names for deal operations, or check pipeline configuration.

List deal (or custom module) pipelines in Zoho CRM with their stages, win probabilities, and display order


## Installation & Usage

To install and use the **Zoho CRM Analytics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-analytics](https://vinkius.com/mcp/zoho-crm-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

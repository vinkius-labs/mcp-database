# Custify MCP Server

Equip your AI agent to manage customer success, monitor health scores, and track churn probability directly via the Custify API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/custify)

## Overview
**Category:** customer-support
**Tools Count:** 10

## Description
Integrate **Custify**, the comprehensive customer success platform, directly into your AI workflow. Monitor customer health, track churn risks, and manage your success tasks and notes using natural language.

### What you can do

- **Customer Oversight** — List and retrieve detailed profiles, health scores, and churn probabilities for all customers.
- **Company Monitoring** — Access company-level metrics and success data to manage B2B relationships effectively.
- **Success Task Management** — List and track open tasks and internal CRM notes for your accounts.
- **KPI Discovery** — Explore key performance indicators and metrics defined in your Custify account.

### How it works

1. Connect the Custify integration to your AI assistant.
2. Authorize using your Custify API Key (found in Settings > API).
3. Optimize your customer success operations through intuitive conversation.

### Who is this for?

- **Customer Success Managers** — Quickly check account health and churn risk on the go.
- **Account Executives** — Retrieve company metrics and recent notes during client reviews.
- **Success Operations** — Audit tasks and KPIs across all customer segments via chat.


## Available Tools
- **create_customer_profile**: Resolves the newly generated customer ID and validation status. Mutates the customer database state.

Create a new customer profile in Custify
- **get_company_details**: Resolves organizational attributes and health metrics. Touches the core company repository.

Get detailed settings and metrics for a specific company
- **get_customer_details**: Resolves health scores, recent activity, and segment membership. Interacts with the behavioral analytics boundary.

Get full profile and health metrics for a specific customer
- **list_companies**: Resolves company IDs, domain information, and association metrics. Touches the account-level organization boundary.

List all companies in Custify
- **list_customers**: Resolves properties such as customer ID, name, email, and lifecycle stage. Interacts with the customer success management boundary.

List all customers in Custify
- **list_customer_kpis**: Resolves metric definitions and threshold values. Interacts with the performance monitoring boundary.

List key performance indicators defined in the account
- **list_customer_notes**: Resolves note content and authorship metadata. Touches the internal communications boundary.

List internal CRM notes for a specific customer
- **list_people**: Resolves contact details and account associations. Touches the relationship management boundary.

List all people associated with accounts
- **list_customer_success_tasks**: Resolves task priority, status, and assigned owners. Interacts with the workflow automation boundary.

List open and completed customer success tasks
- **search_customers_by_keyword**: Resolves matching customer profiles based on name or email. Touches the search and indexing boundary.

Search for customers by name or email


## Installation & Usage

To install and use the **Custify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/custify](https://vinkius.com/mcp/custify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Expensya MCP Server

Submit and approve business expenses in seconds with receipt scanning, policy enforcement, and reimbursement workflows.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/expensya)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Connect your **Expensya** account to any AI agent and take full control of your business spending and automated expense reporting through natural conversation.

### What you can do

- **Expense Orchestration** — List and manage all business expenses programmatically, including retrieving detailed metadata and creating new entries with comments
- **Report Oversight** — Monitor the status of expense reports (Draft, Pending Approval) and access project allocations for high-fidelity financial tracking
- **Organizational Visibility** — Retrieve complete directories of users, categories, and payment methods to coordinate team-wide spending policies
- **Logistics Intelligence** — List and manage vehicles for mileage tracking and monitor supported currencies for international business operations
- **Financial Export** — Programmatically trigger exports of expense data using predefined Export IDs for seamless integration with your accounting tools

### How it works

1. Subscribe to this server
2. Retrieve your **Expensya Token** (Administration > Integrations > API Keys)
3. Obtain your **Ocp-Apim-Subscription-Key** from the Expensya Developer Portal
4. Start managing your expenses from Claude, Cursor, or any MCP client

No more manual entry of every coffee receipt. Your AI acts as your dedicated finance and expense coordinator.

### Who is this for?

- **Finance Teams** — instantly retrieve organizational spending reports and monitor approval queues using natural language
- **Business Travelers** — quickly log new expenses and check project budgets without opening the web dashboard
- **Accountants** — automate the extraction of financial records and audit mileage logs through simple AI queries


## Available Tools
- **create_new_expense**: Requires amount, currency, and category.

Add a new expense record
- **export_expense_data**: Export expenses to a specific format
- **get_authenticated_user_profile**: Get current user profile
- **list_expense_categories**: g., Meals, Travel).

List active expense categories
- **list_supported_currencies**: List all supported currencies
- **list_expenses**: Supports filtering by date, user, and status.

List all business expenses
- **list_payment_methods**: g., Cash, Company Card) configured.

List defined payment methods
- **list_analytical_projects**: List projects for tracking
- **list_expense_reports**: List expense reports (folders)
- **list_expense_tags**: List active tags
- **list_expensya_users**: List users in the organization
- **list_mileage_vehicles**: List vehicles for mileage tracking


## Installation & Usage

To install and use the **Expensya** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expensya](https://vinkius.com/mcp/expensya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

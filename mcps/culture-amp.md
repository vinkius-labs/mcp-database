# Culture Amp MCP Server

Equip your AI agent to manage employee engagement surveys, monitor performance, and track development via the Culture Amp API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/culture-amp)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Culture Amp**, the leading employee experience platform, directly into your AI workflow. Monitor organizational health, track engagement survey progress, and manage employee data using natural language.

### What you can do

- **Employee Management** — List and retrieve detailed profiles for all employees in the platform.
- **Engagement Insights** — Monitor active and past engagement surveys and their participation status.
- **Organizational Structure** — Explore teams and groups defined within Culture Amp to understand your company layout.
- **Analytics Discovery** — List available analytics datasets and demographics for reporting segmentation.

### How it works

1. Connect the Culture Amp integration to your AI assistant.
2. Authorize using your Culture Amp API Key (found in your organization settings).
3. Optimize your employee experience strategy through intuitive conversation.

### Who is this for?

- **People & HR Operations** — Quickly audit employee records and monitor survey participation rates.
- **Team Leads** — Retrieve team-specific data and track engagement trends within their departments.
- **Internal Communications** — Identify engagement gaps and plan outreach based on real-time survey status.


## Available Tools
- **create_employee_record**: Resolves newly created user IDs and verification status. Mutates the employee directory state.

Add a new employee to the Culture Amp platform
- **get_survey_details**: Resolves participant counts and survey settings. Touches the analytics data-source boundary.

Get configuration and status for a specific survey
- **get_employee_details**: Resolves full profile attributes. Touches the core employee information system.

Get detailed profile for a specific employee
- **list_cultureamp_accounts**: Resolves account IDs and organizational scopes. Touches the account management boundary.

List accounts associated with your organization
- **list_analytics_datasets**: Resolves dataset identifiers and types. Touches the reporting data-warehouse boundary.

List available analytics datasets for reporting
- **list_demographic_fields**: Resolves demographic field names and identifiers. Touches the metadata and segmentation boundary.

List demographics used for reporting segments
- **list_organizational_groups**: Resolves group IDs, names, and hierarchical classifications. Touches the organizational mapping boundary.

List groups and teams defined in Culture Amp
- **list_engagement_surveys**: Resolves survey IDs, titles, and lifecycle statuses (active, closed). Interacts with the feedback analytics boundary.

List all engagement and experience surveys
- **list_employees**: Resolves properties such as user ID, email, and employee status. Interacts with the employee directory boundary.

List all employees in Culture Amp
- **search_employees_by_name**: Resolves matched employee profiles. Touches the search and discovery boundary.

Search for employees by name or email keyword


## Installation & Usage

To install and use the **Culture Amp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/culture-amp](https://vinkius.com/mcp/culture-amp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

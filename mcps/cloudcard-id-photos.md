# CloudCard ID Photos MCP Server

Manage ID photo submissions, approvals, and cardholder data via CloudCard directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudcard-id-photos)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Empower your AI agent with access to the **CloudCard** (RemotePhoto) platform to automate your ID card production and photo approval workflows.

### What you can do

- **Photo Approval Workflow**. List submitted photos and approve or deny them with specific reason codes directly through natural language.
- **Cardholder Management**. Register new people (students/employees) and retrieve detailed profile and submission history.
- **Submission Standards**. Access organization-level photo requirements and dimensions to ensure high-quality ID production.
- **Operational Oversight**. Monitor event webhooks, check API health status, and retrieve distribution office locations.

### How it works

1. Subscribe to this server
2. Enter your CloudCard API Token (X-Auth-Token)
3. Start managing your ID production from Claude, Cursor, or any MCP client

### Who is this for?

- **University Registrar Offices**. Quickly approve student ID photos and check submission statuses via natural conversation.
- **Corporate HR Teams**. Manage employee photo uploads and card production without leaving your workspace.
- **Security & Access Control**. Automate cardholder registration and monitor photo requirements using natural language commands.


## Available Tools
- **approve_id_photo**: Approve a submitted photo
- **check_api_health**: Verify CloudCard API connectivity
- **register_new_cardholder**: Requires email and first/last name.

Add a new person to CloudCard
- **deny_id_photo**: Requires a reason code or message for the cardholder.

Deny a submitted photo
- **get_authenticated_profile**: Get current API user info
- **get_organization_settings**: Get organization metadata
- **get_cardholder_details**: Get details for a specific person
- **list_card_offices**: List distribution locations
- **list_cardholders**: List all cardholders (people)
- **list_submitted_photos**: Supports filtering by status.

List all photo submissions
- **list_photo_requirements**: g., format, size, background).

Get submission requirements
- **list_configured_webhooks**: List active event webhooks


## Installation & Usage

To install and use the **CloudCard ID Photos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudcard-id-photos](https://vinkius.com/mcp/cloudcard-id-photos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Retool MCP Server

Connect your AI assistant to Retool to inspect applications, audit users, review connected resources, and monitor workflows directly from chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/retool)

## Overview
**Category:** superpower
**Tools Count:** 7

## Description
Connect your conversational assistant directly to the **Retool** ecosystem. This integration enables your AI to explore the organizational structure of your internal tools, auditing who has access to what, and reviewing which databases are connected.

### What you can do

- **Audit Applications** — Ask your assistant to scan your Retool workspace (`list_apps`) and drill down into the configuration of specific tools (`get_app`). Observe how tools are organized by requesting a view of the folder hierarchy (`list_folders`).
- **Manage Permissions & Users** — Review the active members of your Retool organization (`list_users`) and understand their access levels by listing the existing permission groups (`list_groups`).
- **Review DevOps & Infrastructure** — Command the AI to inspect which data sources or APIs are wired into your operational stack (`list_resources`), and list any active background automation tasks (`list_workflows`).

### How it works

1. Install the Retool extension module in your MCP environment.
2. Obtain your `Retool Access Token` and your `Retool Domain` from your network settings. Enter them securely below.
3. Converse naturally: "List all our active Retool users and tell me if we have any database resources connected."

### Who is this for?

- **IT Administrators** — Run quick audits of internal user privileges and database connections without diving into several clicks in the Retool dashboard.
- **Engineering Leads** — Monitor the landscape of internal tools and workflows directly while chatting about operations.
- **Data Teams** — Quickly verify if the relevant PostgreSQL database has been integrated to Retool for team usage.


## Available Tools
- **get_app**: Retrieves details for a specific Retool application
- **list_apps**: Lists all applications in the Retool organization
- **list_folders**: Lists all folders in the Retool workspace
- **list_groups**: Lists all permission groups
- **list_resources**: Lists all data resources configured in Retool
- **list_users**: Lists all users in the Retool organization
- **list_workflows**: Lists all Retool Workflows


## Installation & Usage

To install and use the **Retool** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retool](https://vinkius.com/mcp/retool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

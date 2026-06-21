# Retool MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retool)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/retool-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/retool-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Connect your AI assistant to Retool to inspect applications, audit users, review connected resources, and monitor workflows directly from chat.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Retool workspace."

**🤖 AI Agent:**
> I invoked `list_users` successfully. I found 8 users in your organization, including `alice@example.com` and `bob@example.com`. Let me know if you need to know their group assignments using the associated permission tools.

---

**👤 You:**
> "List all applications currently configured."

**🤖 AI Agent:**
> Running `list_apps`, I retrieved a total of 12 distinct internal tools within your environment. Popular examples include your 'Admin Dashboard', 'Customer Refund Portal', and 'Inventory Tracker'. Would you like the detailed properties for a specific one?

---

**👤 You:**
> "Tell me what resources are connected to our Retool."

**🤖 AI Agent:**
> By querying `list_resources`, I can see 5 integrated services in your Retool account. This includes your production 'PostgreSQL Database', a 'Stripe API' connector, and an 'S3 Bucket' for file uploads. The connections are confirmed active.


## Installation & Usage

To install and use the **Retool** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retool](https://vinkius.com/mcp/retool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

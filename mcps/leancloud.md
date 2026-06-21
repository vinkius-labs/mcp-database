# LeanCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leancloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/leancloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/leancloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scalable backend-as-a-service platform — manage data classes, users, and push notifications via AI.

## Description
Empower your AI agent to orchestrate your entire backend infrastructure with **LeanCloud**, the premier backend-as-a-service platform for modern developers. By connecting LeanCloud to your agent, you transform complex data modeling, user management, and notification delivery into a natural conversation. Your agent can instantly list data objects, retrieve detailed record metadata, manage user profiles, and even initiate push notifications without you ever needing to navigate the comprehensive LeanCloud console. Whether you are conducting a data audit or monitoring application usage, your agent acts as a real-time backend assistant, keeping your data accurate and your services responsive.

### What you can do

- **Data Orchestration** — List and retrieve detailed information about objects in any of your LeanCloud data classes.
- **User Management** — Browse and retrieve user profiles to audit your application's membership base.
- **Content Control** — Create, update, and delete data objects programmatically through the agent interface.
- **File Auditing** — Browse and list files uploaded to your application's cloud storage.
- **Push Notifications** — Initiate and monitor push notification deliveries to engage your users instantly.

### How it works

1. Subscribe to this server
2. Enter your LeanCloud App ID and App Key
3. Start managing your backend through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — automate data maintenance and monitor application health through natural language queries.
- **Product Operations** — manage user records and coordinate push notifications directly from your AI-powered workspace.
- **Data Analysts** — retrieve system records and audit application statistics via a unified AI interface.
- **LeanCloud Power Users** — integrate your existing backend workflows into your AI-driven daily routines.


## Available Tools
- **create_object**: Create a new object
- **delete_object**: Delete an object
- **get_app_stats**: Get application statistics
- **get_object**: Get object details
- **get_user**: Get user details
- **list_files**: List application files
- **list_objects**: List objects in a class
- **list_users**: List application users
- **push_notification**: Send push notification
- **update_object**: Update an object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LeanCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 objects in the 'GameScore' class."

**🤖 AI Agent:**
> I've retrieved the latest records from the GameScore class. You have 5 recent entries, including scores from 'User8821' and 'User9920'. Would you like to view the full metadata for the highest score?

---

**👤 You:**
> "Show me all users in the application."

**🤖 AI Agent:**
> I've listed the users for your LeanCloud application. You have 150 total registered members. Should I retrieve the detailed profile for the most recently active user?

---

**👤 You:**
> "Check the application statistics for today."

**🤖 AI Agent:**
> I've retrieved the app statistics. Today, your backend has handled 5,000 API requests with a 99.9% success rate. Storage usage is currently at 1.2GB. Would you like a breakdown of the most called endpoints?


## Installation & Usage

To install and use the **LeanCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leancloud](https://vinkius.com/mcp/leancloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

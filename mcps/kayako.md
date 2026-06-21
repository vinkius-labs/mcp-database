# Kayako MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kayako)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kayako-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kayako-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage support tickets, users, and knowledge base articles via Kayako — list cases, create users, and browse help center content directly from any AI agent.

## Description
Connect your **Kayako** helpdesk to any AI agent to streamline your customer support and knowledge management workflows through natural conversation.

### What you can do

- **Case Management** — List support cases, create new conversations, and retrieve all posts/messages within a specific case ID.
- **User & Organization Insights** — List users and organizations, create new user profiles, and fetch details for the currently authenticated agent.
- **Team Collaboration** — Explore team structures, list all configured teams, and identify members within specific support groups.
- **Knowledge Base Access** — Browse Help Center articles and categories to quickly find documentation or support resources.
- **Workflow Optimization** — Access macros and custom views to understand how support queues are organized and automated.

### How it works

1. Subscribe to this server
2. Enter your Kayako Domain and API Access Token
3. Start managing support tickets and customer data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — monitor case volumes, inspect specific ticket threads, and manage team assignments without leaving the chat interface.
- **Customer Success Managers** — quickly look up user profiles and organization history to provide personalized assistance.
- **Technical Writers** — verify Help Center article listings and categories directly from their workspace.


## Available Tools
- **list_article_comments**: List comments for a specific Kayako article
- **list_articles**: List Kayako Help Center articles
- **list_brands**: List Kayako brands
- **list_case_posts**: List posts for a specific Kayako case
- **list_cases**: Supports pagination and partial output.

List Kayako cases (conversations)
- **list_categories**: List Kayako Help Center categories
- **create_case**: Create a new Kayako case
- **create_file**: Upload a file to Kayako
- **create_user**: Create a new Kayako user
- **list_endpoints**: List Kayako automation endpoints
- **list_locales**: List Kayako locales
- **list_macros**: List Kayako macros
- **get_me**: Get current Kayako user details
- **list_monitors**: List Kayako automation monitors
- **list_organizations**: List Kayako organizations
- **list_sections**: List Kayako Help Center sections
- **list_team_members**: List members of a specific Kayako team
- **list_teams**: List Kayako teams
- **list_triggers**: List Kayako automation triggers
- **list_users**: Supports pagination and partial output.

List Kayako users
- **list_views**: List Kayako views


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kayako** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent support cases in Kayako."

**🤖 AI Agent:**
> I've retrieved the latest cases. You have 3 open tickets: 'Login Issue' (ID: 450), 'Billing Inquiry' (ID: 451), and 'Feature Request' (ID: 452). Would you like to see the details for any of these?

---

**👤 You:**
> "Show me all members of the 'Technical Support' team."

**🤖 AI Agent:**
> Fetching team members for ID 12... The 'Technical Support' team currently includes: Alice Smith, Bob Jones, and Charlie Brown.

---

**👤 You:**
> "List all available views in our Kayako instance."

**🤖 AI Agent:**
> I found several configured views: 'All Open Cases', 'My Assigned Tickets', 'Pending Customer Response', and 'Recently Completed'. Which one would you like to explore?


## Installation & Usage

To install and use the **Kayako** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kayako](https://vinkius.com/mcp/kayako)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

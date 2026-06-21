# Apiary MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apiary)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apiary-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apiary-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your API design-first workflows via Apiary — read blueprints, publish docs, and run tests directly from your AI agent.

## Description
Connect your **Apiary** workspace to your AI agent and take full control of your API design, specification, and validation processes through natural conversation.

### What you can do

- **Read API Blueprints** — Fetch raw Markdown-based API Blueprints or Swagger files defining endpoints, methods, and parameters without leaving your editor
- **Publish Documentation** — Instantly update your Apiary projects with new markdown code. Mock servers and public documentation sync automatically
- **Run Dredd Tests** — Validate your backend implementation against the blueprint specifications using integrated tests
- **Team Management** — Query team API projects, list team members, and manage your engineering ecosystem intuitively

### How it works

1. Subscribe to this server
2. Enter your Personal Apiary Token
3. Start querying your APIs or instruct Claude/Cursor to refactor endpoints instantly

No copying and pasting back and forth to the Apiary browser editor.

### Who is this for?

- **Backend Engineers** — ask your assistant to fetch the current blueprint, write new endpoint specifications, and publish them back automatically
- **Technical Writers** — easily review and fix API documentation formatting and submit changes directly to the remote server
- **Engineering Managers** — list all active APIS under your team, oversee member permissions, and check the testing status


## Available Tools
- **list_apis**: Apiary is an API design-first platform.

List all API projects on Apiary
- **get_api**: Get the full API Blueprint source code of an Apiary API project
- **publish_blueprint**: Use with valid Markdown blueprint/Swagger.

Publish (update) the API Blueprint of an Apiary API project
- **get_me**: Get the authenticated Apiary user profile
- **list_team_apis**: List all API projects belonging to a specific Apiary team
- **list_teams**: List all teams the authenticated user belongs to on Apiary
- **get_team**: Get details of a specific Apiary team
- **list_team_members**: List all members of an Apiary team
- **run_tests**: Get or run Dredd-style API tests against an Apiary project
- **get_doc_url**: Get the documentation and mock server URLs for an Apiary API project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apiary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the API Blueprint code for my project named 'payments-gateway'."

**🤖 AI Agent:**
> Here is the raw Markdown blueprint from 'payments-gateway'. It currently has 15 endpoints categorized under 'Transactions' and 'Refunds'. How would you like me to modify it?

---

**👤 You:**
> "List all team members of the 'frontend-team' in Apiary."

**🤖 AI Agent:**
> I've fetched the member list for 'frontend-team'. There are 4 members associated with this workspace, including 1 admin and 3 regular publishers. Would you like to check what APIs this team owns?

---

**👤 You:**
> "Update my 'users-api' with this new blueprint code..."

**🤖 AI Agent:**
> I have successfully published the updated markdown code to 'users-api'. Apiary has verified the syntax to be valid Blueprint, and the mock server along with the documentation URL has been refreshed automatically.


## Installation & Usage

To install and use the **Apiary** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apiary](https://vinkius.com/mcp/apiary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Mokaform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mokaform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mokaform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mokaform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create interactive forms and surveys with visual logic builders that adapt questions based on previous answers dynamically.

## Description
Connect your **Mokaform** account to any AI agent and manage AI-powered forms through natural conversation.

### What you can do

- **Form Management** — Create, update, and list forms
- **Response Collection** — Browse and read form submissions
- **Workspace Management** — Organize forms across multiple workspaces
- **Response Actions** — View individual responses or delete them

### How it works

1. Subscribe to this server
2. Enter your Mokaform API Key
3. Start managing forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Teams** — collect user feedback and feature requests
- **HR** — manage job applications and onboarding forms
- **Marketers** — build lead capture and survey forms


## Available Tools
- **create_form**: Create a new form
- **delete_response**: Delete a form response
- **get_form**: Get form details
- **get_response**: Get specific response details
- **list_forms**: List all forms
- **list_responses**: List all responses for a form
- **list_workspaces**: List all workspaces
- **update_form**: Update an existing form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mokaform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms and show their response counts."

**🤖 AI Agent:**
> Forms: 4. 1) 'Customer Feedback' (ID: frm_123, 145 responses). 2) 'Job Application' (ID: frm_456, 23 responses). 3) 'Event RSVP' (ID: frm_789, 89 responses). 4) 'Feature Request' (ID: frm_012, 34 responses). Workspace: 'Default'.

---

**👤 You:**
> "Show the latest 3 responses for the Customer Feedback form."

**🤖 AI Agent:**
> Latest responses (frm_123): 1) Sarah T. — Rating: 5/5, Comment: 'Love the new dashboard!' (2h ago). 2) Mike L. — Rating: 3/5, Comment: 'Onboarding could be faster.' (5h ago). 3) Lisa R. — Rating: 4/5, Comment: 'Great support team!' (1d ago).

---

**👤 You:**
> "Create a new feedback form in the Marketing workspace."

**🤖 AI Agent:**
> Form created! ✅ Title: 'Product Feedback Q2'. ID: frm_345. Workspace: 'Marketing'. Status: Draft. Ready to add fields and publish.


## Installation & Usage

To install and use the **Mokaform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mokaform](https://vinkius.com/mcp/mokaform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

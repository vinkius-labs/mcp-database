# Userback MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/userback)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/userback-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/userback-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Collect visual feedback from users with annotated screenshots, screen recordings, and bug reports embedded in your product.

## Description
Connect your **Userback** account to any AI agent and simplify how you collect and manage visual feedback, bug reports, and user suggestions through natural conversation.

### What you can do

- **Feedback Management** — List all feedback entries and retrieve detailed metadata, screenshots, and comments for specific reports.
- **Project Control** — List and query feedback projects to keep your development and design work organized.
- **Direct Creation** — Programmatically create new feedback entries or bug reports for specific projects via AI.
- **Team Visibility** — List account users and collaborators to understand your organization's review team.
- **Status Tracking** — Monitor the progress of feedback items and verify if issues have been resolved.

### How it works

1. Subscribe to this server
2. Enter your Userback API Token (found in your account settings under API)
3. Start managing your visual feedback from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers & Designers** — quickly retrieve user feedback and verify visual bugs via simple AI commands.
- **QA & Support Teams** — monitor incoming reports and create feedback entries directly from the workspace.
- **Development Leads** — coordinate bug fixes and track feedback status across multiple projects.


## Available Tools
- **create_feedback_entry**: Create a new feedback entry
- **get_feedback_details**: Get details for a specific feedback
- **get_project_details**: Get details for a specific project
- **list_feedbacks**: List Userback feedbacks
- **list_userback_projects**: List Userback projects
- **list_account_users**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Userback** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all feedback projects in my Userback account."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active feedback spaces: 'Marketing Site', 'Product App v2', and 'Internal Tools'. Which one would you like to see feedback for?

---

**👤 You:**
> "Show me the latest bug reports for the 'Product App v2' project."

**🤖 AI Agent:**
> I've fetched the entries. There are 4 recent reports including 'Login button overlap', 'Checkout error on mobile', and 'Missing icon in settings'. Shall I retrieve details for the checkout error?

---

**👤 You:**
> "Create a new suggestion: 'Add dark mode support' to project '10293'."

**🤖 AI Agent:**
> Success! The suggestion 'Add dark mode support' has been created for project 10293 (ID: fb_99023). I've added your notes and it is now visible in your dashboard.


## Installation & Usage

To install and use the **Userback** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/userback](https://vinkius.com/mcp/userback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

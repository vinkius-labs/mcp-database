# Good Grants MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/good-grants)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/good-grants-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/good-grants-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Discover and manage grant applications with a platform that matches your organization to the right funding opportunities.

## Description
Connect your **Good Grants** account to any AI agent and simplify how you coordinate your grant programs, track applicant data, and monitor the review process through natural conversation.

### What you can do

- **Application Oversight** — List all grant applications and retrieve detailed metadata, status, and custom field values.
- **Review & Scoring** — List and query application reviews and scores to monitor the evaluation progress.
- **Fund Management** — List available grant funds and programs to coordinate your funding distribution.
- **User & Applicant CRM** — Manage your directory of users and team members registered in the system.
- **Categorization** — List and query grant categories to organize your programs and maintain a structured database.
- **Operational Automation** — Create new grant applications programmatically and verify configurations via AI commands.
- **Real-time Status** — Check the progress of individual applications and verify reviewer assignments directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Good Grants API Key (found in your account settings)
3. Start managing your grant lifecycle from Claude, Cursor, or any MCP client

### Who is this for?

- **Program Managers & Grant Officers** — quickly check application statuses and monitor scoring progress via simple AI queries.
- **Operations Teams** — manage fund distributions and verify applicant metadata directly from the workspace.
- **Reviewers & Evaluators** — verify assigned applications and retrieve review history via the AI assistant.


## Available Tools
- **create_new_application**: Register a new application
- **get_application_details**: Get details for a specific application
- **list_applications**: List Good Grants applications
- **list_grant_categories**: List grant categories
- **list_grant_funds**: List grant funds
- **list_application_reviews**: List reviews
- **list_account_users**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Good Grants** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active grant applications in my account."

**🤖 AI Agent:**
> I've retrieved your applications. You have 25 active submissions including 'Community Garden Project', 'Tech for Good Grant', and 'Startup Seed Fund'. Which one would you like to see the details or status for?

---

**👤 You:**
> "Show me the reviews and scores for application 'app_10293'."

**🤖 AI Agent:**
> Fetching reviews... For application app_10293, I found 3 reviews with an average score of 8.5/10. Reviewers highlighted the 'Social Impact' as a strong point. Shall I retrieve the full comments?

---

**👤 You:**
> "Create a new application titled 'Youth Tech Workshop' in the 'Education' category."

**🤖 AI Agent:**
> Success! The application 'Youth Tech Workshop' has been created in your Good Grants account (ID: app_88231). It is currently in draft status in the 'Education' category.


## Installation & Usage

To install and use the **Good Grants** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/good-grants](https://vinkius.com/mcp/good-grants)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

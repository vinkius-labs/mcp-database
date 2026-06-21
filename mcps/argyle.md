# Argyle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/argyle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/argyle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/argyle-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Verify employment and income with Argyle — track users, employments, and payouts via AI.

## Description
The **Argyle MCP Server** brings automated employment and income verification directly to your AI agent. Seamlessly manage your user verification workflows, retrieve detailed employment history, and monitor income totals using simple natural language.

### Key Capabilities

- **User Management** — List all users in your Argyle account and create new unique user IDs for verification flows.
- **Employment Verification** — Retrieve verified employment status, hire dates, job titles, and employer details from the source.
- **Income Analysis** — Access detailed income totals and breakdown, including YTD, monthly, and per-pay-period data.
- **Payout Tracking** — List individual pay period details (payouts) to understand gross/net pay and deductions.
- **Verified Identities** — Retrieve verified name, address, and contact information directly from payroll sources.
- **Secure Data Access** — Uses secure API keys and supports sandbox mode for safe testing and production usage.

### Who is this for?

- **Lenders & Underwriters** — Quickly verify applicant income and employment status without manual document collection.
- **HR & Compliance Teams** — Audit employee data and monitor verification progress using AI-assisted commands.
- **Fintech Developers** — Integrate payroll data retrieval into your automated financial products and services.


## Available Tools
- **create_user**: Create a new user in Argyle
- **get_account_check**: Verify Argyle account connection
- **get_employment**: Retrieve employment history for a specific user
- **get_income**: Retrieve income totals and breakdown for a user
- **list_identities**: Retrieve verified identity information for a user
- **list_payouts**: List individual pay period details (payouts) for a user
- **list_users**: List all users created in your Argyle account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Argyle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in my Argyle account."

**🤖 AI Agent:**
> I've retrieved your user list. You have 50 users registered for verification, including recent IDs 'user_abc123' and 'user_xyz789'.

---

**👤 You:**
> "Show me the employment history for user 'user_12345'."

**🤖 AI Agent:**
> User 'user_12345' is currently employed as a 'Senior Developer' at 'TechCorp', with a hire date of Jan 15, 2020.

---

**👤 You:**
> "What is the total YTD income for user 'user_abc'?"

**🤖 AI Agent:**
> The total YTD income for user 'user_abc' is $45,200.50, based on 12 verified payouts from their payroll source.


## Installation & Usage

To install and use the **Argyle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/argyle](https://vinkius.com/mcp/argyle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

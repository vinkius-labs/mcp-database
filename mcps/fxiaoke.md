# Fxiaoke MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fxiaoke)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fxiaoke-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fxiaoke-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Leading sales management and CRM platform in China — manage leads, opportunities, and approvals via AI.

## Description
Empower your AI agent to orchestrate your sales operations with **Fxiaoke** (纷享销客), the premier sales management and CRM platform in China. By connecting Fxiaoke to your agent, you transform complex pipeline tracking, lead management, and approval workflows into a natural conversation. Your agent can instantly list your leads, retrieve sales tasks, monitor approval statuses, and even audit team activity without you ever needing to navigate the complex Fxiaoke dashboard. Whether you are managing high-volume leads or complex B2B approval chains, your agent acts as a real-time sales operations assistant, keeping your CRM data accurate and your team aligned.

### What you can do

- **Lead & Opportunity Tracking** — List all active leads and sales opportunities to maintain a clear picture of your pipeline.
- **Sales Task Management** — Monitor and manage sales tasks and activities to keep your team productive.
- **Approval Workflow Monitoring** — List recent approval instances and retrieve detailed status information for rapid coordination.
- **Account & Contact Control** — Browse companies and individual contacts within your CRM ecosystem.
- **Team Overview** — Access organization user lists to manage assignments and participation effectively.

### How it works

1. Subscribe to this server
2. Enter your Fxiaoke App ID, App Secret, and Permanent Code
3. Start managing your sales operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Directors** — monitor overall pipeline health, audit approval chains, and track team velocity through natural language.
- **Sales Operations Managers** — coordinate leads and update CRM records directly from your AI-powered workspace.
- **Business Analysts** — retrieve CRM data for market performance analysis and sales reporting.
- **Fxiaoke Power Users** — integrate your existing CRM workflows into your AI-driven daily routines.


## Available Tools
- **create_lead**: Create a new Fxiaoke lead
- **create_opportunity**: Create a new Fxiaoke opportunity
- **get_approval_details**: Get approval details
- **list_accounts**: List Fxiaoke accounts
- **list_approvals**: List approval instances
- **list_contacts**: List Fxiaoke contacts
- **list_leads**: List Fxiaoke leads
- **list_opportunities**: List Fxiaoke opportunities
- **list_sales_tasks**: List Fxiaoke sales tasks
- **list_users**: List Fxiaoke users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fxiaoke** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads in my Fxiaoke CRM."

**🤖 AI Agent:**
> I've retrieved your active leads from Fxiaoke. You have 85 leads in total, with 12 currently marked as 'Hot'. Which one would you like more details on?

---

**👤 You:**
> "Check the status of recent approval requests."

**🤖 AI Agent:**
> I've listed the recent approvals. There are 5 instances pending, including 2 for 'Discount Authorization' and 1 for 'Contract Sign-off'. Would you like the details for any specific instance?

---

**👤 You:**
> "Create a new lead for 'Mario' with mobile '13800000000'."

**🤖 AI Agent:**
> Done! I've created a new lead record for 'Mario' in Fxiaoke. I've also recorded the mobile number. Would you like to add a company name or source info?


## Installation & Usage

To install and use the **Fxiaoke** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fxiaoke](https://vinkius.com/mcp/fxiaoke)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

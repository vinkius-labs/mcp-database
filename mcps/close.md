# Close MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/close)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/close-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/close-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage sales and pipelines via Close CRM — track leads, monitor opportunities, and manage tasks directly from any AI agent.

## Description
Connect your **Close** CRM account to any AI agent and take full control of your sales automation through natural conversation. Streamline how you manage leads, deals, and daily to-dos natively.

### What you can do

- **Lead Oversight** — List and retrieve details for all leads (companies) including status and contact info natively
- **Opportunity Intelligence** — Access and monitor sales deals and their values across different pipelines flawlessly
- **Task Management** — List and review CRM tasks and reminders to stay on top of your follow-ups securely
- **Pipeline Logistics** — Monitor sales pipelines and understand where deals are in the funnel flawlessly
- **Status Tracking** — List available stages for leads and opportunities to maintain clean data flawlessly
- **User Visibility** — Access your own profile and core CRM metadata directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your Close API Key (found in Settings > API Keys)
3. Start managing your sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — monitor deal progress and review lead history using natural language
- **Sales Managers** — audit pipeline health and team task lists without opening the dashboard
- **Account Executives** — quickly look up lead details and historical opportunity values straight from their chat interface
- **Revenue Ops** — verify lead status mapping and monitor sales throughput


## Available Tools
- **get_lead_details**: Get detailed information for a specific lead
- **get_my_close_profile**: Retrieve information about the authenticated user
- **get_opportunity_details**: Get detailed information for a specific opportunity
- **list_lead_statuses**: List available stages/statuses for leads
- **list_close_leads**: List all leads in Close CRM
- **list_close_opportunities**: List all sales opportunities
- **list_close_pipelines**: List sales pipelines configured in the account
- **list_close_tasks**: List CRM tasks and reminders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Close** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 leads in Close."

**🤖 AI Agent:**
> Retrieving your recent leads... I found 5 items: 'Acme Corp' (Interested), 'TechFlow' (Potential), 'Global Dist' (Qualified), and 2 others. Would you like to see the contacts for Acme?

---

**👤 You:**
> "Show me the value of my current sales pipeline."

**🤖 AI Agent:**
> Calculating pipeline value... Across all active opportunities, your current pipeline value is $125,000. Most deals are in the 'Discovery' stage ($80,000).

---

**👤 You:**
> "What are my pending tasks for this week?"

**🤖 AI Agent:**
> Checking your tasks... You have 12 pending tasks this week, including 5 follow-up calls, 3 contract reviews, and 4 email responses. Should I list the high-priority ones?


## Installation & Usage

To install and use the **Close** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/close](https://vinkius.com/mcp/close)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

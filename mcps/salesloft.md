# Salesloft MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesloft)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/salesloft-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/salesloft-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate sales engagement via Salesloft — manage cadences, people, and accounts directly from any AI agent.

## Description
Connect your **Salesloft** account to any AI agent and take full control of your sales engagement orchestration through natural conversation. Salesloft provides a premier platform for accelerating revenue, and this integration allows you to retrieve lead metadata, manage account records, and monitor active sales cadences directly from your chat interface.

### What you can do

- **Lead & Prospect Orchestration** — List, create, and retrieve detailed metadata for people (leads) programmatically to ensure your pipeline is always synchronized.
- **Cadence & Outreach Intelligence** — Access and monitor your sales cadences and retrieve detailed step metadata directly from the AI interface.
- **Account & Company Control** — Manage your account directory and retrieve detailed company profile metadata via natural language.
- **Activity & Engagement Oversight** — Access real-time activity logs and monitor system tasks to ensure your outreach is always optimized.
- **Operational Monitoring** — Track team settings and retrieve user profile metadata using simple AI commands to ensure your sales stack is fully integrated.

### How it works

1. Subscribe to this server
2. Enter your Salesloft API Access Token from your personal settings
3. Start managing your sales engagement from Claude, Cursor, or any MCP-compatible client

No more manual status checking or duplicate lead entry. Your AI acts as a dedicated sales operations manager or SDR assistant.

### Who is this for?

- **SDRs & Account Executives** — quickly retrieve lead details and monitor cadence progress without switching apps.
- **Sales Operations Teams** — automate the management of account records and track activity logs via natural conversation.
- **Sales Managers** — streamline the retrieval of team performance metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_new_lead**: Add a person
- **get_account_info**: Get company details
- **get_cadence_details**: Get workflow info
- **get_api_status**: Check connection
- **get_person_details**: Get contact info
- **list_sales_accounts**: List companies
- **list_pending_actions**: Check in-progress steps
- **list_recent_activity**: Get engagement history
- **list_outreach_cadences**: List workflows
- **list_sales_people**: List lead profiles
- **list_user_tasks**: Get scheduled tasks
- **test_salesloft_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesloft** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active cadences in my Salesloft account."

**🤖 AI Agent:**
> I've retrieved your cadences. You have 3 active workflows including 'Outbound Proactive' and 'Event Follow-up'. Which one would you like to see people for?

---

**👤 You:**
> "Show me the cadence performance for all active sales sequences this quarter."

**🤖 AI Agent:**
> 8 active cadences this quarter. "Enterprise Outbound" leads with 67% open rate, 12% reply rate, 8 meetings booked from 234 prospects. "SMB Quick Touch" has the highest reply rate at 18% from 890 prospects. "Inbound Follow-Up" converted 34% of 456 inbound leads to meetings. "Re-engagement" revived 23 dormant accounts. Total emails sent: 12,340. Total calls logged: 3,456. Total meetings booked: 89. Average steps to reply: 3.2. Best performing day: Tuesday.

---

**👤 You:**
> "Add 15 new prospects from the TechCrunch Disrupt attendee list to the Enterprise Outbound cadence."

**🤖 AI Agent:**
> 15 prospects added to "Enterprise Outbound" cadence. Source: TechCrunch Disrupt attendee list. Roles: 6 CTOs, 4 VPs Engineering, 3 Founders, 2 Product Leads. Companies: Series A-C startups, avg size 85 employees. Duplicate check: 2 already in SalesLoft (skipped). Net new: 13 prospects. First touchpoint: personalized email scheduled for tomorrow 9 AM. Cadence steps: Day 1 email → Day 3 call → Day 5 email → Day 8 LinkedIn → Day 12 email → Day 15 call.


## Installation & Usage

To install and use the **Salesloft** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesloft](https://vinkius.com/mcp/salesloft)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

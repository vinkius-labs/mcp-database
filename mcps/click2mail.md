# Click2Mail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/click2mail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/click2mail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/click2mail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage physical mail and printing via Click2Mail — track jobs, monitor credit balance, and submit mailings directly from any AI agent.

## Description
Connect your **Click2Mail** account to any AI agent and take full control of your physical mailing and printing operations through natural conversation. Streamline how you manage letters, postcards, and certified mail natively.

### What you can do

- **Job Oversight** — List and retrieve details for all physical mail printing and mailing jobs natively
- **Cost Intelligence** — Access estimated costs for mail jobs before submission to manage budgets flawlessly
- **Asset Logistics** — List uploaded documents and address lists available for your mailing campaigns securely
- **Order Automation** — Submit mail jobs for production and delivery directly from your chat interface flawlessly
- **Credit Tracking** — Retrieve your current account credit balance for mailing flawlessly
- **Activity Auditing** — Access a history of account activities and transactions directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Click2Mail Username and Password
3. Start managing your physical mail from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — automate physical mail workflows and verify job statuses using natural language
- **Marketing Teams** — audit direct mail campaign costs and asset availability without opening the dashboard
- **Finance Teams** — quickly look up transaction history and credit balances straight from their chat interface
- **Customer Support** — verify status of certified mail and individual recipient deliveries


## Available Tools
- **get_mail_credit_balance**: Retrieve the current account credit balance for mailing
- **get_mail_job_cost**: Retrieve the estimated cost for a mail job before submission
- **get_mail_job_details**: Get detailed information for a specific mail job
- **get_mail_account_history**: Retrieve a history of account activities and transactions
- **list_mail_address_lists**: List uploaded address lists available for mailing
- **list_mail_documents**: List uploaded documents available for mailing
- **list_mail_jobs**: List all physical mail printing and mailing jobs
- **submit_mail_job**: Submit a mail job for production and delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Click2Mail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active mail jobs in Click2Mail."

**🤖 AI Agent:**
> Retrieving your mail jobs... I found 3 items: 'Monthly Invoices' (In Production), 'New Year Postcards' (Mailed), and 'Service Notice' (Pending). Would you like the tracking for the postcards?

---

**👤 You:**
> "What is the cost for job ID 98765?"

**🤖 AI Agent:**
> Checking cost for job 98765... The total estimated cost is $42.50 ($12.50 for printing and $30.00 for postage). You have enough credit to submit this job.

---

**👤 You:**
> "Show me my current mailing credit balance."

**🤖 AI Agent:**
> Checking account balance... You currently have $150.75 in mailing credits available. This can be used for any future physical mailing jobs.


## Installation & Usage

To install and use the **Click2Mail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/click2mail](https://vinkius.com/mcp/click2mail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

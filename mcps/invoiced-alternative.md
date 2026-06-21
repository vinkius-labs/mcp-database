# Invoiced MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/invoiced-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/invoiced-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/invoiced-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Get paid faster with automated invoicing, smart payment reminders, and accounts receivable workflows that reduce DSO.

## Description
Connect your **Invoiced** account to any AI agent and take full control of your accounts receivable orchestration and automated billing workflows through natural conversation.

### What you can do

- **Invoice Portfolio Orchestration** â€” List and manage all issued invoices programmatically, retrieving detailed payment metadata and aging statuses
- **Customer & Payment Intelligence** â€” Programmatically retrieve directories of customers and access complete credit profiles and payment history in real-time
- **A/R Workflow Architecture** â€” Access your complete directory of payment plans and auto-pay settings to coordinate your organizational revenue
- **Operational Monitoring** â€” Access real-time status updates for paid invoices and track collection metrics directly through your agent for instant reporting
- **Infrastructure Verification** â€” Verify account-level API connectivity and monitor transaction volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Invoiced dashboard (Settings > API)
3. Start orchestrating your revenue growth from Claude, Cursor, or any MCP client

No more manual following up on overdue payments or missing billing updates. Your AI acts as your dedicated finance coordinator and accounts receivable architect.

### Who is this for?

- **Finance Managers** â€” instantly retrieve invoice summaries and monitor collection goals using natural language commands
- **Accounts Receivable Leads** â€” verify individual customer metadata and track payment history without leaving your creative workspace
- **Developers** â€” integrate high-speed Invoiced billing data into custom ERP and accounting pipelines through simple AI queries


## Available Tools
- **check_invoiced_status**: Verify Invoiced API connectivity
- **create_customer**: Create a customer
- **create_invoice**: Pass line items as JSON array with name, quantity, and unit_cost.

Create an invoice
- **get_customer**: Get customer details
- **get_invoice**: Get invoice details
- **list_credit_notes**: List all credit notes
- **list_customers**: List all customers
- **list_estimates**: List all estimates
- **list_invoices**: List all invoices
- **list_payments**: List all payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoiced** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all unpaid invoices in my Invoiced account."

**🤖 AI Agent:**
> You have 7 unpaid invoices totaling ,450. The largest is INV-1042 for ,200 (due in 3 days). Would you like to see the customer details or send a payment reminder?

---

**👤 You:**
> "Create an invoice for customer 5001 with 2 items."

**🤖 AI Agent:**
> Invoice INV-1098 created for customer 5001. Total:  (Web Design: , SEO Audit: ). The invoice is ready to send. Would you like to add a due date?

---

**👤 You:**
> "List all estimates waiting for approval."

**🤖 AI Agent:**
> You have 4 pending estimates totaling ,000. The oldest is EST-0034 (,500) sent 12 days ago. Would you like to follow up with the customer?


## Installation & Usage

To install and use the **Invoiced** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/invoiced-alternative](https://vinkius.com/mcp/invoiced-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

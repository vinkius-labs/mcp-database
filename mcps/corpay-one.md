# Corpay One MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corpay-one)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/corpay-one-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/corpay-one-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Simplify business payments with automated AP processing, virtual cards, and vendor management that saves your finance team hours.

## Description
Connect your **Corpay One** business payment account to any AI agent and simplify how you pay bills, manage vendor relationships, and monitor your financial documents through natural conversation.

### What you can do

- **Payment Oversight** — List all processed and scheduled bill payments and retrieve detailed reconciliation metadata.
- **Document Management** — Query your catalog of scanned or uploaded invoices and receipts with full data extraction details.
- **Vendor CRM** — List all registered vendors and suppliers to manage your procurement network effectively.
- **Financial Insights** — Check the real-time status of individual payments and documents directly from the agent.
- **Team Coordination** — List account users and team members to understand organizational distribution.
- **Workflow Automation** — Upload new document metadata and initiate financial records via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Corpay One API Key (found in your account settings under API)
3. Start managing your business payments from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Managers & Controllers** — quickly check payment statuses and verify invoice data via simple AI queries.
- **Accounts Payable Teams** — monitor vendor directories and track document approval flows directly from the workspace.
- **Business Owners** — get instant bird's-eye views of company spending and upcoming bill payments via the AI assistant.


## Available Tools
- **create_new_document**: Upload a new document
- **get_document_details**: Get details for a specific document
- **get_payment_details**: Get details for a specific payment
- **list_financial_documents**: List invoices and receipts
- **list_payments**: List Corpay One payments
- **list_team_users**: List account users
- **list_account_vendors**: List vendors/suppliers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corpay One** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recent bill payments."

**🤖 AI Agent:**
> I've retrieved your payments history. You have 3 recent payments including #PAY-10293 ($1,250.00 to AWS), #PAY-10294 ($450.00 to Staples), and 1 scheduled payment. Which one would you like more details on?

---

**👤 You:**
> "Show me the details for invoice 'doc_88231'."

**🤖 AI Agent:**
> Fetching document... Invoice doc_88231 is from 'Cloud Solutions Ltd' for the amount of $2,400.00 USD. It was uploaded on Dec 1st and is currently 'Awaiting Approval'. Would you like the full breakdown?

---

**👤 You:**
> "List all vendors in my account."

**🤖 AI Agent:**
> Retrieving vendors... You have 15 registered suppliers including 'Amazon Business', 'Google Cloud', 'Local Office Supplies', and 'Utility Co'. Shall I check the latest payments for any specific vendor?


## Installation & Usage

To install and use the **Corpay One** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corpay-one](https://vinkius.com/mcp/corpay-one)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

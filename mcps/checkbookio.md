# Checkbook.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkbookio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkbookio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkbookio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage digital and physical check payments via Checkbook — send money, track checks, and monitor invoices directly from any AI agent.

## Description
Connect your **Checkbook.io** account to any AI agent and take full control of your push payments and digital checks through natural conversation. Streamline how you disburse funds to vendors and contractors.

### What you can do

- **Payment Oversight** — List and retrieve details for all digital and physical checks sent or received natively
- **Send Money** — Issue new digital checks via email/phone or physical checks via mail flawlessly
- **Account Intelligence** — Access linked bank accounts and monitor their verification status securely
- **Invoice Management** — List and retrieve details for all invoices within your account flawlessly
- **Recurring Payments** — Monitor and manage active check payment subscriptions securely
- **Profile Visibility** — Retrieve core user profile metadata and account settings directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkbook API Key and API Secret (obtained from Developer Settings)
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Accounts Payable Teams** — automate the disbursement of checks to vendors using natural language
- **Small Business Owners** — send digital checks and monitor balances without opening the bank portal
- **Payroll Administrators** — quickly verify check statuses and payment histories straight from their chat interface
- **Logistics Managers** — track physical checks sent via mail to contractors


## Available Tools
- **get_check_details**: Get detailed information for a specific check
- **get_checkbook_profile**: Retrieve core user profile information
- **list_linked_bank_accounts**: List all bank accounts linked to the profile
- **list_checkbook_checks**: io.

List all digital and physical checks
- **list_checkbook_invoices**: List all invoices
- **list_recurring_payments**: List all recurring check payment subscriptions
- **send_digital_check**: Send a digital check to a recipient via email or phone
- **send_physical_check**: Send a physical check to a recipient via mail


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkbook.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 checks in Checkbook."

**🤖 AI Agent:**
> Retrieving your recent checks... I found 5 items: $100.00 to John Doe (Paid), $250.00 to Acme Inc (In Process), and 3 others. Would you like to see the details for any of these?

---

**👤 You:**
> "Send a digital check for $50 to 'sarah@example.com' with memo 'Refund'."

**🤖 AI Agent:**
> Issuing digital check... The check for $50.00 has been sent to sarah@example.com. The check ID is 'chk_123456'.

---

**👤 You:**
> "Show me my linked bank accounts."

**🤖 AI Agent:**
> Checking your linked banks... You have 2 accounts connected: 'Chase Checking (****1234)' and 'Wells Fargo Savings (****5678)'. Both are verified and ready for use.


## Installation & Usage

To install and use the **Checkbook.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkbookio](https://vinkius.com/mcp/checkbookio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

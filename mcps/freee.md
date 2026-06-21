# freee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freee-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage Japanese accounting and business via freee — track deals and invoices, handle partners and expenses, and audit tax codes directly from any AI agent.

## Description
Connect your **freee** (Accounting/HR) account to any AI agent and take full control of your Japanese business operations and general ledger through natural conversation.

### What you can do

- **Accounting Deal Orchestration** — Extract explicit general ledger accounting entries including income, expense, and journal boundaries mapped to your Company ID natively
- **Invoice State Auditing** — Retrieve explicitly attached invoice statuses (sent, unsent, paid, overdue) to resolve your tenant's Accounts Receivable limits limitlessly
- **Partner & Address Book Control** — Enumerate official business counterparts linking precise vendor, customer, and tax ID profiles synchronously
- **Expense Management** — Analyze explicit expense claims submitted by employees and track managerial approval states before final settlement flawlessly
- **Financial Account Oversight** — Identify connected physical bank accounts, credit cards, and offline cash repositories tracked in your freee instance securely
- **Tax Compliance Mapping** — Execute bulk iterations tracking explicitly registered Japanese Tax mappings evaluating 8%, 10%, and reduced rates synchronously
- **Deal Detail Inspection** — Fetch strict sub-entry details for specific deals to view settlement flags and connected bank sync boundaries natively

### How it works

1. Subscribe to this server
2. Enter your freee Access Token and Company ID (found in freee Developer Console and Business Settings)
3. Start managing your Japanese business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners in Japan** — monitor company cash flow and audit invoices without navigating the freee web UI
- **Accounting Teams** — verify tax code mappings and manage business partner records using natural language
- **Ops Managers** — track employee expense applications and verify settlement statuses in real-time
- **Developers** — test and debug Japanese accounting API integrations and verify financial schemas through natural conversation


## Available Tools
- **list_deals**: List all accounting deals (transactions)
- **get_deal**: Get deal details
- **list_partners**: List all business partners
- **get_partner**: Get partner details
- **list_accounts**: List all account items
- **list_walletables**: List bank accounts and wallets
- **list_taxes**: List tax codes
- **list_invoices**: List all invoices
- **list_expenses**: List expense applications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **freee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 accounting deals in freee"

**🤖 AI Agent:**
> Retrieving deals... I found 5 recent transactions including an income entry from 'Client A' (¥150,000) and an expense for 'Office Rent' (¥80,000). Would you like to see the settlement details for any of these?

---

**👤 You:**
> "Show me pending expense applications"

**🤖 AI Agent:**
> Analyzing expenses... There are 3 applications pending managerial approval: 'Taxi Fare' from John, 'Client Lunch' from Sarah, and 'Stationery' from Mike. I can provide the receipts and total amounts for you.

---

**👤 You:**
> "What are my active bank accounts in freee?"

**🤖 AI Agent:**
> Checking wallets... You have 3 connected accounts: 'MUFG Main' (¥2,500,000), 'Corporate Visa' (-¥120,000), and 'Petty Cash' (¥50,000). The MUFG account was last synced 2 hours ago.


## Installation & Usage

To install and use the **freee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freee](https://vinkius.com/mcp/freee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

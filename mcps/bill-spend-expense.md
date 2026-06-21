# BILL Spend & Expense MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bill-spend-expense)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bill-spend-expense-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bill-spend-expense-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage corporate spend via BILL — list budgets, cards, and transactions directly from any AI agent.

## Description
Connect your **BILL Spend & Expense (formerly Divvy)** account to any AI agent and orchestrate your corporate spending through natural conversation.

### What you can do

- **Budget Oversight** — List and inspect active budgets to track spending against limits.
- **Card Management** — View virtual and physical cards assigned to employees.
- **Transaction Auditing** — Retrieve real-time transactions and merchant data.
- **User Management** — List employees and review their roles.
- **Reimbursement Tracking** — Check the status of out-of-pocket expense claims.

### How it works

1. Subscribe to this server
2. Enter your BILL Spend API Token
3. Start managing your expenses from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **list_budgets**: List all budgets
- **list_cards**: List all cards
- **list_reimbursements**: List all reimbursements
- **list_transactions**: List recent transactions
- **list_users**: List all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BILL Spend & Expense** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active budgets."

**🤖 AI Agent:**
> I've retrieved your budgets. You have 'Marketing Q2' and 'Engineering Software' budgets.

---

**👤 You:**
> "Show recent transactions."

**🤖 AI Agent:**
> Retrieving transactions... I found 5 recent charges, including AWS ($150) and Uber ($25).

---

**👤 You:**
> "List pending reimbursements."

**🤖 AI Agent:**
> You have 2 pending reimbursements for 'Team Lunch' and 'Conference Travel'.


## Installation & Usage

To install and use the **BILL Spend & Expense** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bill-spend-expense](https://vinkius.com/mcp/bill-spend-expense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

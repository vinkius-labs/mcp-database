# Confido Legal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/confido-legal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/confido-legal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/confido-legal-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage legal trust accounting, client payments, and compliance reporting with tools built specifically for law firms.

## Description
Connect your **Confido Legal** account to any AI agent and take full control of your law firm's financial operations and trust-compliant payment workflows through natural conversation.

### What you can do

- **Payment Orchestration** — Create and manage professional payment links programmatically, including splitting funds between trust and operating accounts in a single transaction
- **Matter & Client Lifecycle** — List and manage legal matters and client profiles programmatically to maintain a high-fidelity record of your firm's caseload and relationships
- **Trust Compliance Intelligence** — Access information about your firm's connected bank accounts to ensure processing fees are never deducted from trust funds
- **Billing Automation** — Programmatically create and retrieve payment link details and monitor recurring subscription plans to streamline your law firm's revenue cycle
- **Account Visibility** — Access high-level firm metadata and transaction histories directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Base URL** from your Confido Legal (Gravity Legal) dashboard
3. Start managing your legal payments and matters from Claude, Cursor, or any MCP client

No more manual entry into split-payment spreadsheets. Your AI acts as your dedicated legal billing coordinator and financial analyst.

### Who is this for?

- **Law Firm Administrators** — instantly retrieve payment link statuses and update client records using natural language commands
- **Attorneys** — generate trust-compliant payment requests for matters without leaving your workspace
- **Legal Tech Developers** — automate billing workflows and monitor transaction histories through simple AI queries


## Available Tools
- **create_client**: Create a new client
- **create_payment_link**: Can split between trust and operating amounts.

Create a new payment link
- **get_firm_details**: Get firm details and bank accounts
- **get_payment_link_details**: Get payment link details
- **list_clients**: List all clients
- **list_matters**: Optionally filter by client ID.

List matters
- **list_payment_links**: List all payment links
- **list_subscriptions**: List all payment subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Confido Legal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment link for client ID 'cl_123': $500 for operating and $1000 for trust."

**🤖 AI Agent:**
> Payment link generated! I've created a split payment link for client cl_123. Total: $1,500.00. Funds will be routed to your Operating ($500) and Trust ($1,000) accounts upon completion. Link: [payment_url].

---

**👤 You:**
> "List all active legal matters for client ID 'cl_123'."

**🤖 AI Agent:**
> I've retrieved the matters for client cl_123. You have 2 active cases: 'Estate Planning 2026' (ID: m_456) and 'Corporate Filing'. Would you like the current trust balance for either of these?

---

**👤 You:**
> "Show my firm's connected bank accounts."

**🤖 AI Agent:**
> Accessing firm metadata... You have 2 connected accounts: 'Business Operating' and 'IOLTA Trust Account'. Both are verified and active for split payments. Shall I check for any pending payouts?


## Installation & Usage

To install and use the **Confido Legal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confido-legal](https://vinkius.com/mcp/confido-legal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

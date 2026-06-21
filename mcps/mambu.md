# Mambu MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mambu)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mambu-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mambu-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage clients, loans, deposits, and tasks on Mambu Cloud Banking Platform.

## Description
The Mambu MCP server allows you to interact with your Mambu tenant. You can list and get details for clients, loan accounts, deposit accounts, transactions, tasks, activities, and communications. This integration uses the Mambu v2 REST API to provide a seamless experience for managing your banking operations. Your token is encrypted at rest and injected securely at runtime.


## Available Tools
- **get_client**: Get details for a specific Mambu client
- **get_deposit_account**: Get details for a specific Mambu deposit account
- **get_loan_account**: Get details for a specific Mambu loan account
- **get_task**: Get details for a specific Mambu task
- **list_activities**: List Mambu activities
- **list_clients**: List Mambu clients
- **list_communications**: List Mambu communications
- **list_deposit_accounts**: List Mambu deposit accounts
- **list_loan_accounts**: List Mambu loan accounts
- **list_tasks**: List Mambu tasks
- **list_transactions**: List Mambu transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mambu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all clients in Mambu"

**🤖 AI Agent:**
> Found 24 clients in Mambu:
1. Acme Corp (ID: 12345) — Active, 3 loan accounts
2. TechVentures (ID: 12346) — Active, 1 savings account
3. GreenEnergy Ltd (ID: 12347) — Active, 2 loan accounts
... Showing 3 of 24.

---

**👤 You:**
> "Show details for client with ID 12345"

**🤖 AI Agent:**
> Client details for ID 12345:
Name: Acme Corp. Status: Active. Created: Jan 15, 2024.
Accounts: 3 loan accounts (total outstanding: $125,000), 1 savings ($8,500 balance).
Risk rating: Low. Last transaction: March 18, 2025.

---

**👤 You:**
> "List my tasks in Mambu"

**🤖 AI Agent:**
> You have 5 pending tasks in Mambu:
1. Review loan application #LA-789 (Due: today)
2. Approve disbursement for Acme Corp (Due: tomorrow)
3. Follow up on overdue payment — Client #12350 (3 days overdue)
4. Complete KYC review — TechVentures (Due: April 5)
5. Monthly portfolio risk report (Due: April 1)


## Installation & Usage

To install and use the **Mambu** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mambu](https://vinkius.com/mcp/mambu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

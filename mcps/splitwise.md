# Splitwise MCP Server

Connect your Splitwise account to AI agents to track expenses, check balances, and manage shared groups.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/splitwise)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
### What you can do
- **Track Expenses:** Give your AI agent the ability to check who owes who across your distinct groups.
- **Log Bills:** Ask your AI to calculate receipts and accurately add the expense directly into Splitwise with automatic percentage or custom splits.
- **Manage Friends & Groups:** Easily pull details of group members.

### How it works
1. Log into your Splitwise account.
2. Navigate to your Developer Applications settings to generate a personal API token.
3. Insert your Splitwise API Key directly into Vinkius vault.

### Who is this for?
Perfect for roommates, travel groups, and everyday individuals using AI tools like Claude/Cursor to parse complex grocery or travel receipts and directly sync them to Splitwise.


## Available Tools
- **create_expense**: Expects a stringified JSON object containing details like cost, description, format details (e.g. users__0__user_id=123, users__0__paid_share=5.00, etc. or JSON).

Create an expense
- **delete_expense**: Delete an expense
- **get_current_user**: Get current user details
- **get_expense**: Get a specific expense
- **get_expenses**: List expenses
- **get_friend**: Get friend details
- **get_friends**: List all friends
- **get_group**: Get group details
- **get_groups**: List all groups
- **get_user**: Get user details by ID


## Installation & Usage

To install and use the **Splitwise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/splitwise](https://vinkius.com/mcp/splitwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

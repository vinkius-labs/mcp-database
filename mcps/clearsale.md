# ClearSale MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearsale)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clearsale-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clearsale-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage e-commerce fraud prevention via ClearSale — submit orders for analysis, monitor fraud scores, and track status updates directly from any AI agent.

## Description
Connect your **ClearSale** account to any AI agent and take full control of your fraud prevention operations through natural conversation. Streamline how you monitor and analyze e-commerce transactions natively.

### What you can do

- **Order Oversight** — Submit detailed order data for real-time fraud scoring and manual analysis natively
- **Status Intelligence** — Access and monitor the current fraud analysis status for any specific order ID flawlessly
- **Manual Logistics** — Update order statuses in ClearSale's system (e.g., Approved, Cancelled) securely
- **History Tracking** — List and review recently analyzed orders to understand fraud trends flawlessly
- **Connectivity Logistics** — Retrieve core account and connectivity metadata directly within your workspace flawlessly
- **Decision Auditing** — Retrieve detailed fraud scores and analysis reasons provided by ClearSale flawlessly

### How it works

1. Subscribe to this server
2. Enter your ClearSale API Username and Password
3. Start managing your fraud prevention from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor fraud rates and review suspicious orders using natural language
- **Fraud Analysts** — audit specific order scores and update decisions without opening the dashboard
- **Finance Teams** — quickly look up order status and verified transactions straight from their chat interface
- **Ops Teams** — verify system connectivity and monitor real-time analysis throughput


## Available Tools
- **get_clearsale_account_info**: Retrieve core account connectivity information
- **get_order_fraud_status**: Retrieve the current fraud analysis status for an order
- **list_recent_fraud_analyses**: List recently analyzed orders
- **submit_order_fraud_analysis**: Submit an order for real-time fraud analysis
- **update_clearsale_order_status**: Update the status of an order in ClearSale (e.g. Cancelled, Approved)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClearSale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the fraud status for order #ped_12345."

**🤖 AI Agent:**
> Retrieving status for order ped_12345... ClearSale has 'Approved' this order with a fraud score of 15. No further manual analysis is required.

---

**👤 You:**
> "List my last 5 fraud analyses."

**🤖 AI Agent:**
> Checking recent analyses... I found 5 orders: 3 Approved, 1 Denied (Score: 95), and 1 in Manual Analysis. Would you like to see the reasons for the denied order?

---

**👤 You:**
> "Mark order #ped_98765 as 'Cancelled' in ClearSale."

**🤖 AI Agent:**
> Updating order ped_98765... The status has been successfully set to 'Cancelled' (CAN) in the ClearSale system.


## Installation & Usage

To install and use the **ClearSale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearsale](https://vinkius.com/mcp/clearsale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

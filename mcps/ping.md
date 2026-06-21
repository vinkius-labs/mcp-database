# Ping++ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ping)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ping-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ping-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Bring unified payment intelligence to your AI with Ping++. Integrate WeChat, Alipay, and UnionPay through a single clean API interface.

## Description
Empower your Agent to seamlessly manage Chinese payment ecosystems with **Ping++**, the ultimate multi-channel payment aggregator. Connect to WeChat Pay, Alipay, UnionPay, and multiple other networks through a single, elegant interface, replacing complex point-to-point integrations.

### What you can do

- **Unified Charges** — Create and manage transactions across any supported payment channel
- **Refund Management** — Process and retrieve refunds across any network without learning specific gateway APIs
- **Customer Synchronization** — Create and track customer profiles and saved payment methods across platforms

### How it works

1. Subscribe to this server
2. Obtain your Secret API Key from your [Ping++ Developer Dashboard](https://dashboard.pingxx.com)
3. Inject the server into your LLM client and instantly manage multi-channel billing flows

### Who is this for?

- **E-Commerce Agents** — Automate refunds, track transaction states, and manage cross-channel payments seamlessly
- **Financial Operators** — Consolidate the management of WeChat and Alipay transactions without touching backend code
- **Developers in China** — Connect multiple SDK backends to a single MCP endpoint to rapid prototype monetization


## Available Tools
- **create_charge**: Requires the order_no, amount, app ID, channel, currency, subject, and body.

Create a new charge (payment request)
- **create_customer**: Create a new Customer
- **create_refund**: Create a refund for a specific charge
- **list_charges**: List existing charges
- **list_customers**: List existing Customers
- **retrieve_charge**: Retrieve the details of an existing charge
- **retrieve_customer**: Retrieve Customer details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ping++** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 successful charges for my Ping++ app."

**🤖 AI Agent:**
> Here are your last 5 incoming charges across all payment channels. Three originated from WeChat Pay (wx_lite) and two from Alipay. Total amount processing: 12500 CNY.

---

**👤 You:**
> "Create a new refund of 100 CNY for charge ID ch_xyz789."

**🤖 AI Agent:**
> I've successfully created the refund for charge `ch_xyz789` (Amount: 10000 cents). The status is currently marked as 'pending' with the downstream payment channel.

---

**👤 You:**
> "Show me the details for customer ID cus_12345."

**🤖 AI Agent:**
> Customer `cus_12345` was created on Oct 12. They have two saved payment methods bound, including one UnionPay source, and an empty balance.


## Installation & Usage

To install and use the **Ping++** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ping](https://vinkius.com/mcp/ping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

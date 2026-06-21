# Swarm MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swarm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/swarm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/swarm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Orchestrate multi-agent AI workflows where specialized agents collaborate, delegate tasks, and solve complex problems together.

## Description
Connect your **Swarm** loyalty account to any AI agent and simplify how you manage customer rewards, award points for transactions, and handle redemptions through natural conversation.

### What you can do

- **Point Management** — Retrieve real-time point balances and loyalty tiers for specific customer IDs.
- **Transaction Processing** — Programmatically award points to customers by registering sale amounts and product data via AI.
- **Reward Redemption** — Convert customer points into discount vouchers or specific rewards and list all active vouchers.
- **Catalog Discovery** — Browse available rewards and check eligibility for specific customers instantly.
- **Voucher Oversight** — List and query all unused discount codes currently assigned to a customer's profile.
- **Loyalty Lifecycle** — Manage the entire customer reward journey directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Swarm API Key (found in your account dashboard)
3. Start managing your loyalty program from your favorite AI assistant

### Who is this for?

- **Retail Business Owners** — quickly check customer points and award rewards during checkout via simple AI commands.
- **Marketing Managers** — monitor reward distribution and verify voucher availability directly from the workspace.
- **Customer Success Teams** — assist customers with point inquiries and handle manual redemptions via the AI assistant.


## Available Tools
- **get_customer_balance**: Check customer loyalty points
- **list_available_rewards**: List redeemable rewards
- **list_customer_vouchers**: List active customer vouchers
- **process_loyalty_transaction**: Process a sale and award points
- **redeem_customer_reward**: Redeem points for a reward


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swarm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the point balance for customer 'cust_10293'?"

**🤖 AI Agent:**
> I've retrieved the balance. Customer cust_10293 currently has 1,250 points and is in the 'Gold Tier'. They are eligible for a 15% discount voucher. Would you like to redeem it now?

---

**👤 You:**
> "Award points for a $150 purchase to customer 'cust_88231'."

**🤖 AI Agent:**
> Transaction processed! I've awarded the points for a $150.00 sale to customer cust_88231. Their new balance is now 1,400 points. The customer has been notified via email.

---

**👤 You:**
> "Show me all available rewards I can claim with 500 points."

**🤖 AI Agent:**
> Fetching reward catalog... With 500 points, you can claim: 'Free Coffee' (200 pts), '10% Discount Code' (400 pts), or 'Sticker Pack' (150 pts). Which one would you like to redeem?


## Installation & Usage

To install and use the **Swarm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swarm](https://vinkius.com/mcp/swarm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

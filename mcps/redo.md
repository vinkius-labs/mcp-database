# Redo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/redo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/redo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/redo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage returns, track shipping protection claims, and oversee exchanges via AI agents with Redo.

## Description
Connect your **Redo** account to any AI agent to automate your returns management and shipping protection workflows through the Model Context Protocol (MCP). Redo provides a comprehensive suite for handling customer returns, exchanges, and package protection claims for lost or damaged items. This MCP server enables you to track return requests, approve claims, and process final resolutions directly through natural conversation.

### Key Features

- **Returns & Claims Oversight** — List all return requests and shipping protection claims, checking their status and customer metadata instantly.
- **Status Automation** — Update the lifecycle status of a return (e.g., approved, rejected) programmatically from your chat interface.
- **Resolution Processing** — Trigger final actions like refunds, store credits, or exchange order creation for lost or damaged packages.
- **Collaborative Notes** — Add internal comments and communication logs to any return or claim record for better team alignment.
- **Coverage Discovery** — Access high-level information about your shipping protection settings and eligible products.
- **Shipping Rate Calculation** — Retrieve real-time shipping rates for return packages to estimate costs for your customers.
- **Webhook Visibility** — Monitor active webhooks to ensure your internal systems are receiving real-time return notifications.
- **Real-time Synchronization** — Keep your post-purchase operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Redo Store ID and API Secret (found in your Redo settings)
3. Start managing your returns and claims from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Ops & Support** — quickly check the status of a customer's claim or approve a return without manual dashboard navigation.
- **Customer Success Teams** — get a real-time overview of recent return reasons and sentiment via simple AI commands.
- **Logistics Managers** — automate the retrieval of shipping rates and monitor protection coverage levels.


## Available Tools
- **add_internal_note**: Post a return comment
- **approve_return_claim**: Approve a request
- **verify_api_connection**: Check connection
- **get_store_details**: Get store metadata
- **get_protection_summary**: Get coverage details
- **get_return_details**: Get return metadata
- **get_return_shipping_rates**: Get shipping costs
- **list_protected_items**: List covered products
- **list_store_returns**: List returns/claims
- **list_return_webhooks**: List webhook configs
- **process_final_resolution**: Finalize return/claim
- **reject_return_claim**: Reject a request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Redo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 pending return requests."

**🤖 AI Agent:**
> Retrieving requests... I found 5 pending returns, including one from 'john@email.com' for 'Reason: Damaged in transit'. Would you like the full details?

---

**👤 You:**
> "Approve the return claim for ID 'ret_abc123'."

**🤖 AI Agent:**
> Claim approved! I have successfully updated the status of return ret_abc123 to 'approved'. The customer will receive their instructions automatically.

---

**👤 You:**
> "Get the shipping rates for return 'ret_abc123'."

**🤖 AI Agent:**
> Calculating rates... I found 3 shipping options for this return. Standard Ground is $8.50 and Express is $15.75. Which one would you like to select?


## Installation & Usage

To install and use the **Redo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redo](https://vinkius.com/mcp/redo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

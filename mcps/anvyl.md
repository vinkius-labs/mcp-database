# Anvyl MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anvyl)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anvyl-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anvyl-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Streamline your supply chain with Anvyl — manage purchase orders, track shipments, and coordinate with suppliers via AI.

## Description
The **Anvyl MCP Server** brings visibility and automation to your supply chain operations. By connecting your Anvyl account to your AI agent, you can seamlessly track production progress, manage parts and suppliers, and update critical milestones using natural language.

### What you can do

- **Order Visibility** — List all purchase orders and drill down into specific order details to check status and quantities.
- **Milestone Management** — Track production and shipping milestones. Confirm completions or record delays directly from your chat.
- **Supplier Coordination** — Quickly retrieve supplier information and part specifications stored in Anvyl.
- **Logistics Tracking** — Access tracking records and logistics data for any purchase order to keep your team informed on delivery timelines.

### How it works

1. Subscribe to this server
2. Provide your Anvyl API Key and Team ID
3. Start managing your supply chain workflow through your AI chat interface.

### Who is this for?

- **Supply Chain Managers** — Automate the tracking of multiple POs and receive instant updates on milestone statuses.
- **Procurement Teams** — Efficiently look up part details and supplier contact information during planning.
- **Operations Leads** — Keep a high-level view of production health and logistics without manually navigating through dashboards.


## Available Tools
- **confirm_milestone**: Confirm a milestone for a purchase order
- **delay_milestone**: Delay a milestone for a purchase order
- **get_part**: Get details for a specific part
- **get_purchase_order**: Get details for a specific purchase order
- **get_supplier**: Get details for a specific supplier
- **list_logistics**: List tracking records for a purchase order
- **list_milestones**: List milestones for a purchase order
- **list_parts**: List parts in the Anvyl account
- **list_purchase_orders**: List Anvyl purchase orders for the team
- **list_suppliers**: List suppliers in the Anvyl account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anvyl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active purchase orders."

**🤖 AI Agent:**
> I've retrieved 12 active purchase orders. The most recent one is PO #8821 for 'Aluminum Housings' with an expected delivery date of April 15th.

---

**👤 You:**
> "Check the milestones for order PO-123."

**🤖 AI Agent:**
> Order PO-123 has 5 milestones. 'Material Sourcing' and 'Production Start' are completed. 'Quality Inspection' is currently in progress and expected by tomorrow.

---

**👤 You:**
> "Delay milestone 'm_456' for order PO-789 by 1 week because of raw material shortage."

**🤖 AI Agent:**
> I've updated the milestone 'm_456' for order PO-789. The new expected date is now set to May 22nd, and the reason 'raw material shortage' has been recorded.


## Installation & Usage

To install and use the **Anvyl** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anvyl](https://vinkius.com/mcp/anvyl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Convertlab MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/convertlab)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/convertlab-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/convertlab-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Marketing automation and customer data platform — manage customers, campaigns, and events via AI.

## Description
Empower your AI agent to orchestrate your marketing operations with **Convertlab** (DM Hub), the leading customer engagement and marketing automation platform in China. By connecting Convertlab to your agent, you transform complex customer segmentation, campaign tracking, and behavioral auditing into a natural conversation. Your agent can instantly list customers, retrieve detailed profile information, monitor marketing campaigns, and browse behavioral events without you ever needing to navigate the comprehensive DM Hub interface. Whether you are conducting a customer data audit or monitoring the performance of a high-volume campaign, your agent acts as a real-time marketing operations assistant, keeping your data accurate and your engagement moving.

### What you can do

- **Customer Orchestration** — List all DM Hub customers and retrieve detailed profile and membership information.
- **Campaign Management** — Browse active and historical marketing campaigns and retrieve detailed performance metadata.
- **Event Auditing** — List and retrieve detailed customer behavioral events to monitor engagement levels.
- **Segmentation Control** — Browse membership groups and identify customer segments for targeted activities.
- **Operations Insights** — Retrieve metadata about your marketing touchpoints and application status.

### How it works

1. Subscribe to this server
2. Enter your Convertlab App ID and App Secret
3. Start managing your marketing lifecycle through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor campaign progress and audit customer segments through natural language queries.
- **Customer Success Teams** — retrieve detailed member profiles and engagement histories directly from your AI-powered workspace.
- **Operations Leads** — oversee marketing touchpoints and system events via a unified AI interface.
- **Convertlab Power Users** — integrate your existing marketing workflows into your AI-driven daily routines.


## Available Tools
- **create_customer**: Create a new customer
- **get_campaign**: Get campaign details
- **get_customer**: Get customer details
- **list_campaigns**: List marketing campaigns
- **list_customers**: List DM Hub customers
- **list_events**: List marketing events
- **list_member_groups**: List customer segments
- **list_touchpoints**: List marketing touchpoints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convertlab** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my DM Hub customers."

**🤖 AI Agent:**
> I've retrieved your Convertlab customers. You have 1,500 total members, including 150 high-value segments marked with loyalty tags. Would you like to view the details of the most recent ones?

---

**👤 You:**
> "Show me the details for campaign 'Spring-2026'."

**🤖 AI Agent:**
> I've retrieved the details for 'Spring-2026'. The campaign is currently active with a 45% conversion rate across 5 target touchpoints. Would you like a breakdown of the behavioral events triggered by this campaign?

---

**👤 You:**
> "List all customer segmentation groups."

**🤖 AI Agent:**
> I've listed your member groups. There are 12 segments defined, including 'Repeat Buyers', 'Inactive-30-Days', and 'VIP-Tier-1'. Which segment would you like to see the member count for?


## Installation & Usage

To install and use the **Convertlab** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/convertlab](https://vinkius.com/mcp/convertlab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

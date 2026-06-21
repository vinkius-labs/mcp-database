# Ortto (formerly Autopilot) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ortto-formerly-autopilot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ortto-formerly-autopilot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ortto-formerly-autopilot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your CDP, customer data, and marketing automations via Ortto — orchestrate journeys natively via AI.

## Description
Connect your **Ortto** account to any AI agent and unify your customer data and marketing automation workflows through natural conversation.

### What you can do

- **Unified Profiles** — Create, update, and search for person and organizational account records across your CDP
- **Activity Orchestration** — Programmatically trigger custom activities to engage users based on real-time events
- **Campaign Auditing** — List audience segments and retrieve performance metrics for your marketing campaigns and journeys
- **Regional Compliance** — Native support for Global, AU, and EU data centers to ensure your data stays where it belongs

### How it works

1. Subscribe to this server
2. Enter your Ortto API Key and specify your Data Region
3. Start managing your customer journeys from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — instantly segment audiences and trigger localized journeys while planning campaign strategy
- **Customer Success Teams** — update person profiles and audit user activity directly from your team's workspace
- **Marketing Engineers** — automate the creation of activities and data mapping from your IDE


## Available Tools
- **create_activity**: Create a custom activity for a person
- **create_person**: Add a new person to Ortto
- **delete_person**: Permanently archive/delete a person
- **get_person**: Get details for a specific person
- **get_subscription**: Get subscription status for an email
- **list_accounts**: List accounts/organizations in Ortto
- **list_audiences**: List audience segments
- **list_campaigns**: List marketing campaigns
- **list_people**: List people in Ortto
- **update_person**: Update an existing person


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ortto (formerly Autopilot)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the person profile for '[email protected]'."

**🤖 AI Agent:**
> I've retrieved the profile for '[email protected]'. They are currently tagged as 'VIP-Customer' and associated with the 'CloudTech' account. Would you like to see their recent activity history?

---

**👤 You:**
> "List all active marketing campaigns in our EU region."

**🤖 AI Agent:**
> I've queried the EU data center. You have 3 active campaigns: 'Summer Sale 2024', 'Newsletter Weekly', and 'Referral Program'. Each has reached over 5,000 users this month. Which one would you like to audit?

---

**👤 You:**
> "Trigger the 'product-demo-requested' activity for [email protected]"

**🤖 AI Agent:**
> The activity 'product-demo-requested' has been successfully triggered for [email protected]. This will initiate the corresponding automation journey in your Ortto instance.


## Installation & Usage

To install and use the **Ortto (formerly Autopilot)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ortto-formerly-autopilot](https://vinkius.com/mcp/ortto-formerly-autopilot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

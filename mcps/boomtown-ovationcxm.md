# BoomTown (OvationCXM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boomtown-ovationcxm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boomtown-ovationcxm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boomtown-ovationcxm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Orchestrate customer journeys via OvationCXM — manage journeys, teams, and support issues directly from any AI agent.

## Description
Connect your **OvationCXM (BoomTown)** account to any AI agent and orchestrate your customer onboarding, support, and journey workflows through natural conversation.

### What you can do

- **Journey Orchestration** — List and retrieve detailed information for customer journeys, stages, and activities.
- **Team & Org Management** — Access and monitor internal and partner support teams and organizations.
- **Issue Tracking** — Query and inspect support cases and issues across the ecosystem.
- **Customer Intelligence** — Retrieve detailed customer profiles and end-user data managed within CXMEngine.
- **Real-time Monitoring** — Audit journey progress and team assignments directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BoomTown API Token and Secret
3. Start managing your customer journeys from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **CX Operations** — quickly check journey statuses and team assignments without manual dashboard searches.
- **Support Managers** — monitor active cases and partner performance straight from their workflow tools.
- **Onboarding Specialists** — verify customer progress through complex multi-stage journeys using natural language.


## Available Tools
- **get_customer**: Get details of a specific customer
- **get_issue**: Get details of a specific issue
- **get_journey**: Get details of a specific journey
- **get_organization**: Get details of a specific organization
- **get_team**: Get details of a specific team
- **list_customers**: List all customers/end-users
- **list_issues**: List all support issues/cases
- **list_journeys**: List all customer journeys
- **list_organizations**: List all organizations
- **list_teams**: List all support teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoomTown (OvationCXM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customer journeys."

**🤖 AI Agent:**
> I've retrieved your journeys. You have 3 active journeys: 'Onboarding - Enterprise A' (ID: j_1), 'Merchant Activation' (ID: j_2), and 'Support Escalation' (ID: j_3).

---

**👤 You:**
> "Show the details for support issue case_99283."

**🤖 AI Agent:**
> Case case_99283 is currently 'Open' and assigned to the 'Tier 2 Technical Support' team. It was created on March 15th and is related to 'Hardware Connectivity'.

---

**👤 You:**
> "List all organizations in my ecosystem."

**🤖 AI Agent:**
> I've retrieved your organizations. Notable members include 'Global Payments Inc.', 'Tech Solutions Ltd.', and 'Retail Hub'. Would you like details for any of them?


## Installation & Usage

To install and use the **BoomTown (OvationCXM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boomtown-ovationcxm](https://vinkius.com/mcp/boomtown-ovationcxm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

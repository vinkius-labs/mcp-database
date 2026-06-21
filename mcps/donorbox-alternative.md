# Donorbox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donorbox-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/donorbox-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/donorbox-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Collect donations and manage fundraising campaigns with recurring giving, peer-to-peer pages, and donor management for nonprofits.

## Description
Connect your **Donorbox** account to any AI agent and take full control of your nonprofit fundraising and donor engagement workflows through natural conversation.

### What you can do

- **Donation Orchestration** — List and manage donations programmatically, including filtering by email or campaign and retrieving detailed transaction metadata
- **Donor CRM** — Create and update donor profiles programmatically to maintain high-fidelity records of your organization's supporters
- **Recurring Plan Lifecycle** — Monitor, pause, resume, or cancel recurring donation subscriptions directly through your agent to streamline supporter management
- **Campaign Intelligence** — Access your complete directory of fundraising campaigns to monitor performance and coordinate outreach in real-time
- **Operational Monitoring** — Check API connectivity and monitor active webhooks directly through your agent for reliable fundraising operations

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Donorbox (Integrations > API & Zapier)
3. Start managing your nonprofit growth from Claude, Cursor, or any MCP client

No more manual status checking or digging through donation tables in the portal. Your AI acts as your dedicated fundraising strategist and donor coordinator.

### Who is this for?

- **Nonprofit Managers** — instantly retrieve donation summaries and check campaign progress using natural language commands
- **Fundraisers** — update donor information and manage recurring subscriptions without leaving your communication tools
- **Operations Leads** — monitor webhook activity and verify API health through simple AI queries


## Available Tools
- **cancel_recurring_plan**: Cancel a recurring donation
- **check_api_health**: Verify Donorbox API connectivity
- **create_new_donor**: Requires first name, last name, and email.

Add a new donor record
- **get_account_profile**: Get authenticated account info
- **list_fundraising_campaigns**: List fundraising campaigns
- **list_donations**: Can be filtered by email, campaign, or amount.

List all donations
- **list_donors**: Can be filtered by name or email.

List all donors
- **list_recurring_plans**: List recurring donation plans
- **list_configured_webhooks**: List active webhooks
- **pause_recurring_plan**: Pause a recurring donation
- **resume_recurring_plan**: Resume a paused recurring donation
- **update_donor_info**: Modify a donor record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donorbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 donations in my Donorbox account."

**🤖 AI Agent:**
> I've retrieved your latest 5 donations. You've received a total of $450 across them, including a $100 gift from 'John Doe' for the 'Winter Fund'. Would you like the transaction metadata for these?

---

**👤 You:**
> "Check recurring plans for donor 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching subscriptions... John Doe (ID: d_123) has 1 active monthly plan for $25.00. The last payment was successful on March 1st. Shall I retrieve their full donation history?

---

**👤 You:**
> "Pause the recurring plan with ID 'pln_456'."

**🤖 AI Agent:**
> Action complete! Recurring plan pln_456 has been successfully paused. The donor will not be charged until the plan is resumed. I've logged this update in your Donorbox history.


## Installation & Usage

To install and use the **Donorbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donorbox-alternative](https://vinkius.com/mcp/donorbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

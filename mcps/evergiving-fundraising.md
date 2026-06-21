# Evergiving Fundraising MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evergiving-fundraising)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/evergiving-fundraising-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/evergiving-fundraising-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage donations, track fundraising campaigns, and monitor field staff via the Evergiving API.

## Description
Integrate **Evergiving**, the powerful platform for fundraising and field marketing, directly into your AI workflow. Manage your donation records and recurring pledges, track active fundraising campaigns and their performance, monitor field staff schedules and locations, and oversee your entire fundraising operation using natural language.

### What you can do

- **Donation Oversight** — List and retrieve detailed information, donor details, and payment statuses for all your pledges and donations.
- **Campaign Intelligence** — Monitor fundraising campaigns, resolving goals, total raised, and real-time conversion rates.
- **Field Management** — Access and monitor fundraiser schedules and assigned locations, ensuring your field teams are optimized.
- **Fundraising Auditing** — Retrieve high-level summaries of donation volume, recurring pledge health, and organizational account health instantly.

### How it works

1. Connect the Evergiving integration to your AI assistant.
2. Authorize using your Evergiving API Key (found in your account settings).
3. Orchestrate your fundraising strategy and field operations through intuitive conversation.

### Who is this for?

- **Fundraising Managers** — Quickly check daily donation totals and campaign progress on the go.
- **Donor Relations Teams** — Research donor history and recurring pledge statuses via chat.
- **Operations Teams** — Monitor field fundraiser schedules and organizational fundraising metadata instantly.


## Available Tools
- **get_evergiving_account_metadata**: Retrieve metadata and limits for your Evergiving account
- **get_campaign_performance_summary**: Get a summary of performance metrics for a specific fundraising campaign
- **get_donation_detailed_data**: Get detailed settings and information for a specific donation or pledge
- **quick_fundraising_volume_audit**: Retrieve a high-level summary of donations, campaigns, and active fundraisers
- **list_fundraising_campaigns**: List all active fundraising campaigns in your account
- **list_fundraising_donations**: List all donations and pledges collected via Evergiving
- **list_field_marketing_schedules**: List all active schedules and locations for field fundraisers
- **list_active_fundraisers**: List all fundraisers and field staff registered in your organization
- **list_pending_payment_donations**: Identify donations that are currently in a "Pending" or "Incomplete" status
- **list_active_recurring_pledges**: Identify donations that are set up as recurring monthly or annual pledges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evergiving Fundraising** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active fundraising campaigns."

**🤖 AI Agent:**
> I've found 3 active campaigns, including 'Spring Clean Water Drive' and 'Winter Shelter Support'. The Clean Water Drive has raised $12,500 so far. Would you like to see the performance stats for this campaign?

---

**👤 You:**
> "Show me the last 5 donations."

**🤖 AI Agent:**
> I've retrieved the 5 most recent donations, including $100 from 'Alice Johnson' and a $50 recurring pledge from 'Robert Smith'. All are currently 'Processing'. Should I pull the donor contact details for Alice Johnson?

---

**👤 You:**
> "What is the schedule for fundraiser 'John Doe' today?"

**🤖 AI Agent:**
> John Doe is scheduled for the 'Downtown Plaza' location today from 9:00 AM to 5:00 PM. They are currently assigned to the 'Children's Health' campaign. Would you like to see their conversion rate for this week?


## Installation & Usage

To install and use the **Evergiving Fundraising** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evergiving-fundraising](https://vinkius.com/mcp/evergiving-fundraising)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

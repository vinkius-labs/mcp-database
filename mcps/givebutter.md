# Givebutter MCP Server

Manage fundraising campaigns, track donations, and oversee donors via AI agents with Givebutter.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/givebutter)

## Overview
**Category:** customer-relationship-management
**Tools Count:** 12

## Description
Connect your **Givebutter** account to any AI agent to automate your fundraising operations and donor management through the Model Context Protocol (MCP). Givebutter is the modern fundraising platform for nonprofits and changemakers. This MCP server enables you to retrieve donation transactions, manage fundraising campaigns, and synchronize donor profiles (contacts) directly through natural conversation.

### Key Features

- **Donation Oversight** — List all donation transactions, fetch detailed metadata including status and timestamps, and monitor your revenue flow instantly.
- **Campaign Management** — Access active fundraising campaigns and events, retrieving detailed configuration and total raised amounts.
- **Donor Synchronization** — Search and list donor profiles, retrieve detailed contact metadata, and programmatically add new donors to your database.
- **Offline Recording** — Record offline donations or external payments programmatically to maintain a unified source of truth for your fundraising.
- **Recurring Plan Monitoring** — List and track configured recurring donation plans to understand long-term donor commitment.
- **Webhook Visibility** — Monitor active webhooks to ensure your internal systems are receiving real-time donation notifications.
- **Real-time Synchronization** — Keep your nonprofit's financial data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Givebutter API Key (found in Settings > Developers > API)
3. Start managing your fundraising from Claude, Cursor, or any MCP client

### Who is this for?

- **Nonprofit Ops & Finance** — quickly check if a large donation has been cleared or list recent successful transactions without manual dashboard navigation.
- **Development Directors** — get a real-time overview of campaign performance and donor activity via simple AI commands.
- **Donor Relations** — verify donor history and synchronize new contacts into your database seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **sync_donor_contact**: Add new donor
- **record_offline_donation**: Log a donation
- **get_account_details**: Get account identity
- **get_campaign_details**: Get campaign metadata
- **get_transaction_details**: Get transaction metadata
- **list_fundraising_campaigns**: List active campaigns
- **list_donor_contacts**: List donor profiles
- **list_recurring_plans**: List recurring plans
- **list_recent_donations**: List last 10 success
- **list_donation_transactions**: List donations
- **list_donation_webhooks**: List webhook configs


## Installation & Usage

To install and use the **Givebutter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/givebutter](https://vinkius.com/mcp/givebutter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

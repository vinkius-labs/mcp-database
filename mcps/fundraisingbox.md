# FundraisingBox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fundraisingbox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fundraisingbox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fundraisingbox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Process online donations, manage donor relationships, and run fundraising campaigns with tools built for European nonprofits.

## Description
Connect your **FundraisingBox** account to any AI agent and manage your nonprofit fundraising operations through natural conversation.

### What you can do

- **Donation Tracking** — List all donations with amounts, donors, campaigns, and payment methods, and filter by campaign
- **Recurring Donations** — Monitor all active recurring donation subscriptions with frequency and status
- **Donor Management** — Browse all donors with contact info, total donated, and donation count; search by name or email
- **Donor History** — Retrieve complete giving history for any donor including amounts, dates, and campaign allocations
- **Campaign Monitoring** — List all fundraising campaigns with goals, progress, and donation statistics
- **Donation Forms** — View all configured donation form widgets
- **Tax Receipts** — Access all generated donation receipts for fiscal reporting
- **Dashboard Analytics** — Retrieve aggregate fundraising metrics: total raised, donor count, campaign performance, and trends

### How it works

1. Subscribe to this server
2. Enter your FundraisingBox API Key from your organization settings
3. Start managing your fundraising from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fundraising Managers** — track donation trends, monitor campaign progress, and review donor engagement without opening the dashboard
- **Donor Relations** — search donors, review giving histories, and prepare personalized outreach
- **Finance Teams** — access donation receipts and reconcile fundraising data for annual reporting


## Available Tools
- **check_fundraisingbox_status**: Verify connectivity
- **get_dashboard**: Get fundraising dashboard
- **get_donation**: Get donation details
- **get_donor_history**: Get donor history
- **get_donor**: Get donor profile
- **get_campaign**: Get campaign details
- **list_donations_by_project**: List donations by campaign
- **list_donations**: List donations
- **list_donors**: List donors
- **list_forms**: List donation forms
- **list_campaigns**: List campaigns
- **list_receipts**: List donation receipts
- **list_recurring_donations**: List recurring donations
- **search_donors**: Search donors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FundraisingBox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the fundraising dashboard and which campaigns are closest to reaching their goals."

**🤖 AI Agent:**
> Fundraising Dashboard: Total raised this year: €248,500. Active donors: 1,842. Average donation: €67.40. Monthly trend: +12% vs last month. Campaign progress: 1) 'Winter Emergency Aid' — €45,000/€50,000 (90%, 3 days left!). 2) 'School Building Fund' — €112,000/€150,000 (74.7%). 3) 'Clean Water Initiative' — €28,500/€100,000 (28.5%, launched 2 weeks ago). 4) 'Annual Gala 2025' — €63,000/€80,000 (78.8%). Would you like to see donations for the nearly-complete campaign?

---

**👤 You:**
> "Search for donor 'Schmidt' and show their complete donation history."

**🤖 AI Agent:**
> Found 2 donors matching 'Schmidt'. 1) Hans Schmidt (donor_1201, hans@example.de) — lifetime giving: €4,280 across 12 donations. 2) Maria Schmidt (donor_1445, maria@example.de) — lifetime giving: €1,850 across 6 donations. Showing history for Hans Schmidt: 2025: €500 (Winter Aid), €200 (Clean Water). 2024: €1,200 (Annual Gala), €800 (School Fund), €350 (Winter Aid), €230 (Clean Water). 2023: €400 (Annual Gala), €300 (School Fund), €300 (emergency). Total: €4,280 across 3 years. Currently has an active recurring donation of €50/month to 'Clean Water Initiative'. Would you like to see Maria's history or generate a tax receipt?

---

**👤 You:**
> "List all recurring donations and identify which ones have been active for more than a year."

**🤖 AI Agent:**
> You have 156 active recurring donations totaling €8,420/month. 89 have been active for more than 12 months (long-term supporters). Top 5 by monthly amount: 1) Corporate Foundation (€500/month, since 2022). 2) Anonymous (€250/month, since 2023). 3) Hans Schmidt (€50/month, since 2024). 4) Green Family Trust (€100/month, since 2021). 5) Dr. Weber (€75/month, since 2023). Total annual recurring revenue: €101,040. Would you like to segment donors by campaign or see which recurring donations were recently paused?


## Installation & Usage

To install and use the **FundraisingBox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fundraisingbox](https://vinkius.com/mcp/fundraisingbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

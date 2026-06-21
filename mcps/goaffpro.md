# Goaffpro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goaffpro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/goaffpro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/goaffpro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage affiliates, track referral orders, and oversee commissions via AI agents with Goaffpro.

## Description
Connect your **Goaffpro** admin account to any AI agent to automate your affiliate marketing and referral program management through the Model Context Protocol (MCP). Goaffpro is a leading affiliate marketing solution that helps Shopify and e-commerce merchants grow their sales through referrals. This MCP server enables you to retrieve affiliate records, track referral orders, manage commissions, and monitor payouts directly through natural conversation.

### Key Features

- **Affiliate Oversight** — List all affiliates in your program, retrieve detailed profile metadata including stats, and programmatically register new affiliates.
- **Referral Tracking** — Access and list all orders attributed to affiliates to understand which partners are driving the most sales.
- **Commission Management** — Retrieve a log of all earned commissions, filtered by status (pending, paid, rejected) to keep your records accurate.
- **Payout Monitoring** — Access a complete list of payments made to affiliates to ensure transparency and timely distributions.
- **Custom Rewards** — Grant custom bonuses or signup rewards to specific affiliates directly from your chat interface.
- **Affiliate Analytics** — Identify your top-performing affiliates and track their lifetime earnings via simple AI commands.
- **Real-time Synchronization** — Keep your referral and affiliate data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Goaffpro API Access Token (found in Settings > Advanced)
3. Start managing your affiliate program from Claude, Cursor, or any MCP client

### Who is this for?

- **Affiliate Managers** — quickly check an affiliate's performance or approve a commission without manual dashboard navigation.
- **E-commerce Store Owners** — get a real-time overview of referral sales and top-performing partners via simple AI commands.
- **Finance & Ops** — automate the retrieval of payout histories and commission logs for auditing and reporting.


## Available Tools
- **verify_api_connection**: Check connection
- **register_new_affiliate**: Add new affiliate
- **grant_affiliate_reward**: g. signup bonus).

Issue bonus reward
- **find_affiliate_by_email**: Search by email
- **get_program_details**: Get program identity
- **get_affiliate_details**: Get affiliate metadata
- **list_program_affiliates**: List all affiliates
- **list_earned_commissions**: List commission events
- **list_referral_orders**: List referral sales
- **list_affiliate_payouts**: List payout history
- **list_top_performers**: List top affiliates
- **list_affiliate_webhooks**: List webhook configs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goaffpro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active affiliates in my program."

**🤖 AI Agent:**
> Retrieving affiliates... I found 5 active partners, including 'Jane Smith' (ID: 123) and 'Growth Blog'. Would you like the performance stats for any of them?

---

**👤 You:**
> "Show me the referral orders for affiliate ID '987'."

**🤖 AI Agent:**
> Fetching referral orders... Affiliate 987 has driven 3 orders today totaling $450.00. All orders are currently 'Paid'.

---

**👤 You:**
> "Grant a $10 bonus to affiliate 'jane@example.com'."

**🤖 AI Agent:**
> Bonus granted! I have successfully issued a $10.00 reward to Jane Smith for 'Exceptional performance'. She will see this in her affiliate dashboard.


## Installation & Usage

To install and use the **Goaffpro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goaffpro](https://vinkius.com/mcp/goaffpro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

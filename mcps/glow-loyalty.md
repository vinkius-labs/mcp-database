# Glow Loyalty MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glow-loyalty)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/glow-loyalty-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/glow-loyalty-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage loyalty members, track point balances, and oversee rewards via AI agents with Glow Loyalty.

## Description
Connect your **Glow Loyalty** (Shopify) account to any AI agent to automate your rewards program management through the Model Context Protocol (MCP). Glow Loyalty is a robust rewards and referral platform designed for modern Shopify merchants. This MCP server enables you to retrieve member point balances, manually adjust points, and redeem rewards directly through natural conversation.

### Key Features

- **Member Oversight** — List all enrolled loyalty members and fetch detailed point balances, tier statuses, and customer metadata instantly.
- **Point Adjustment** — Manually add or subtract points from a member's balance programmatically from your chat interface, perfect for custom rewards or apologies.
- **Reward Redemption** — Initiate reward redemptions for members, deducting points and generating unique discount codes for your storefront.
- **Campaign Discovery** — List all available rewards configured in your program to understand point requirements and active offers.
- **Tier Tracking** — Monitor member progress across different loyalty tiers to identify and reward your most valuable customers.
- **Program Analytics** — Access high-level metadata for your connected Glow account to verify connectivity and account health.
- **Real-time Synchronization** — Keep your loyalty and retention data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Glow API Key and API Secret (found in Settings > API Key)
3. Start managing your loyalty program from Claude, Cursor, or any MCP client

### Who is this for?

- **Shopify Store Owners** — quickly check a customer's point balance or gift bonus points without manual dashboard navigation.
- **Customer Support Teams** — get a real-time overview of a member's loyalty status and redeem rewards via simple AI commands.
- **Retention Managers** — automate the retrieval of member lists and tier distributions for targeted outreach.


## Available Tools
- **gift_points_to_member**: Gift bonus points
- **adjust_member_points**: Use positive numbers to add, negative to subtract.

Add/remove points
- **verify_api_connection**: Check connection
- **get_reward_spec**: Check reward points
- **find_loyalty_member**: Search member
- **get_program_details**: Get account identity
- **get_member_balance**: Check member points
- **list_members_by_page**: Paginated members
- **list_loyalty_members**: List all members
- **list_new_members**: List latest signups
- **list_available_rewards**: List reward options
- **redeem_loyalty_reward**: Redeem a reward


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glow Loyalty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the point balance for 'customer@email.com'?"

**🤖 AI Agent:**
> Checking points... The customer has 1,250 points and is currently in the 'Gold' tier. They have 2 available rewards they can redeem.

---

**👤 You:**
> "Add 100 bonus points to 'jane@example.com' for social sharing."

**🤖 AI Agent:**
> Points adjusted! I've successfully added 100 points to Jane's balance. Her new total is 550 points.

---

**👤 You:**
> "List all available rewards I can offer to my customers."

**🤖 AI Agent:**
> Retrieving rewards... I found 3 active offers: '$5 Off' (500 pts), '10% Discount' (1000 pts), and 'Free Shipping' (750 pts).


## Installation & Usage

To install and use the **Glow Loyalty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glow-loyalty](https://vinkius.com/mcp/glow-loyalty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

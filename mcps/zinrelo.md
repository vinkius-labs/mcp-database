# Zinrelo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zinrelo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zinrelo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zinrelo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage loyalty programs, reward points, and customer engagement via the Zinrelo API.

## Description
Connect your **Zinrelo** account to any AI agent to automate your loyalty and rewards operations. This MCP server enables your agent to interact with loyalty members, award points for activities or purchases, and manage reward redemptions directly from natural language.

### What you can do

- **Member Management** — Enroll new customers and retrieve detailed loyalty profiles, including tier status and point balances
- **Points Automation** — Award points for custom activities or purchase transactions instantly
- **Reward Processing** — Redeem points for rewards and manage manual point deductions when necessary
- **Activity Auditing** — List comprehensive transaction histories for any loyalty member to track earnings and usage
- **Program Oversight** — Access high-level loyalty settings and account configuration details

### How it works

1. Subscribe to this server
2. Enter your Zinrelo Partner ID and API Key
3. Start managing your loyalty program from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Monitor loyalty member growth and award points for special campaigns via natural language
- **Customer Support** — Quickly check a customer's point balance or transaction history during interactions
- **E-commerce Owners** — Automate the enrollment of new members and tracking of reward activities


## Available Tools
- **award_points_activity**: Award points for a custom activity
- **award_points_purchase**: Award points for a purchase
- **enroll_member**: Enroll or update a loyalty member
- **deduct_points**: Manually deduct points from a user
- **get_member_details**: Get details for a specific loyalty member
- **redeem_reward**: g., coupon).

Redeem points for a reward
- **get_loyalty_settings**: Get account loyalty settings
- **list_member_transactions**: List transaction history for a member
- **list_loyalty_members**: List all loyalty program members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zinrelo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the loyalty profile for 'customer@example.com'."

**🤖 AI Agent:**
> I've retrieved the profile for customer@example.com. They are currently in the 'Gold' tier with 1,250 available points. Would you like to see their recent transactions?

---

**👤 You:**
> "Award 500 points to 'jane.doe@example.com' for a $50.00 purchase."

**🤖 AI Agent:**
> Successfully awarded points for the purchase. Jane Doe now has a total of 1,750 points in her Zinrelo loyalty account.

---

**👤 You:**
> "List all transactions for 'john.smith@example.com'."

**🤖 AI Agent:**
> I found 8 transactions for John Smith. Recent activity includes +100 pts for 'Newsletter Signup' and -500 pts for 'Redeem $5 Coupon'.


## Installation & Usage

To install and use the **Zinrelo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zinrelo](https://vinkius.com/mcp/zinrelo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

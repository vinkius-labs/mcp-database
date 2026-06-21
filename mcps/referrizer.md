# Referrizer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/referrizer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/referrizer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/referrizer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate referral marketing and loyalty via Referrizer — manage contacts, referrals, and rewards directly from any AI agent.

## Description
Connect your **Referrizer** account to any AI agent and simplify your referral marketing, customer loyalty, and retention workflows through natural conversation.

### What you can do

- **Contact Management** — List all customers and contacts, retrieve detailed profile metadata, and monitor loyalty points and status
- **Referral Tracking** — Access a history of successful and pending customer referrals to understand your word-of-mouth growth
- **Campaign Control** — Query past and active marketing automation campaigns to monitor your outreach performance
- **Loyalty Rewards** — List available rewards and incentives to choose the right context for each interaction
- **Direct Enrollment** — Register new contacts and customers programmatically directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Referrizer API Key from your account settings
3. Start managing your referral engine from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_campaign**: Get details for a referral campaign
- **get_referral**: Get details for a specific referral
- **get_reward**: Get details for a specific reward
- **list_transactions**: List all reward transactions
- **create_contact**: Register a new contact
- **get_contact_details**: Get details for a specific contact
- **list_marketing_campaigns**: List marketing campaigns
- **list_contacts**: List Referrizer contacts
- **list_referral_history**: List referrals
- **list_loyalty_rewards**: List available rewards
- **update_contact**: Update a contact profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Referrizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in Referrizer."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 100 active customers, including 'John Doe' (Points: 500) and 'Alice Smith'.

---

**👤 You:**
> "Show me the ROI analysis for all active loyalty and referral campaigns."

**🤖 AI Agent:**
> 5 active campaigns analyzed. "Buy 10 Get 1 Free" has the highest ROI at 340% (cost: $2,400 in free products, revenue generated: $10,560). "Refer a Friend $20" ROI: 280% (cost: $1,800, new customer revenue: $6,840). "Birthday Rewards" ROI: 190% (drives 67% visit rate vs 12% for non-birthday contacts). "Points Program" has 2,340 active members with $34,000 monthly spend. "Check-In Rewards" increased visit frequency by 23%. Total loyalty-driven revenue: $58,400.

---

**👤 You:**
> "Create a new contact and enroll them in the Birthday Rewards campaign."

**🤖 AI Agent:**
> Contact created: Maria Santos. Phone: +1-555-0198. Email: maria.santos@email.com. Birthday: August 15. Enrolled in "Birthday Rewards" campaign. She will receive a $15 birthday reward 3 days before August 15. Also auto-enrolled in "Welcome New Member" sequence (first visit reward: 10% off). Points balance: 0. Loyalty tier: Bronze. First check-in tracked. SMS opt-in confirmed. Next touchpoint: welcome email in 2 hours.


## Installation & Usage

To install and use the **Referrizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/referrizer](https://vinkius.com/mcp/referrizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

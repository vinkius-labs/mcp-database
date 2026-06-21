# PartnerStack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/partnerstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/partnerstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/partnerstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage affiliate and partner programs via PartnerStack — list partners, track leads, and monitor rewards directly from any AI agent.

## Description
Connect your **PartnerStack** account to any AI agent and take full control of your partnership and ecosystem workflows through natural conversation.

### What you can do

- **Partner Oversight** — List all partners and retrieve detailed metadata to manage your ecosystem relationships.
- **Lead Tracking** — List and retrieve details for leads submitted by your partners to monitor the sales pipeline.
- **Customer Management** — List customers associated with specific partners to understand attribution.
- **Reward Monitoring** — List generated rewards and payouts to ensure your partners are incentivized correctly.
- **Campaign & Group Analysis** — List partner groups and campaigns to maintain a clear view of your program structure.

### How it works

1. Subscribe to this server
2. Enter your PartnerStack API Key
3. Start managing your partnership program directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Partnership Managers** — quickly check the status of a specific partner or review recent leads.
- **Channel Operations** — monitor rewards and payouts while auditing program performance.
- **Sales Teams** — lookup customer attribution and partner metadata without leaving your workflow.


## Available Tools
- **get_partner_customer**: Get details for a specific customer
- **get_partner**: Get details for a specific partner
- **list_partner_campaigns**: List all partner campaigns
- **list_partner_customers**: List all customers associated with partners
- **list_partner_groups**: List all partner groups
- **list_partner_leads**: List all leads submitted by partners
- **list_partners**: List all partners
- **list_partner_rewards**: List all generated rewards
- **list_partner_transactions**: List all partner transactions
- **list_partner_webhooks**: List all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PartnerStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active partners in my account."

**🤖 AI Agent:**
> I've retrieved 15 active partners, including 'Referral King', 'Global Affiliates', and 'Tech Connect'. Would you like details for any specific partner?

---

**👤 You:**
> "Show me the last 5 leads submitted by our partners."

**🤖 AI Agent:**
> I've fetched the latest leads. Recent submissions include 'John Smith' from partner 'AffiliateOne' and 'Acme Corp' from 'Growth Partners'. Would you like the full details?

---

**👤 You:**
> "What is the status of the rewards for the 'Summer Campaign'?"

**🤖 AI Agent:**
> I've retrieved the rewards log. For the 'Summer Campaign', there are 12 rewards 'pending_approval' and 8 'paid' rewards. Would you like a list of the pending ones?


## Installation & Usage

To install and use the **PartnerStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/partnerstack](https://vinkius.com/mcp/partnerstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Donately MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donately-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/donately-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/donately-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage Donately fundraising and donor data using AI agents.

## Description
### What you can do
- Retrieve and list incoming donations.
- Manage and list your fundraising campaigns.
- Access donor information and contacts.
- Keep track of recurring subscriptions and peer-to-peer fundraisers.

### How it works
1. Subscribe to Donately.
2. Insert your API Token and Account ID.
3. Let the AI Agent fetch and manage your fundraising data.

### Who is this for?
Ideal for non-profits, NGOs, and fundraising teams who want to seamlessly query their Donately data through AI Agents.


## Available Tools
- **create_donation**: Create a new donation
- **get_campaign**: Get details of a specific campaign
- **get_donation**: Get details of a specific donation
- **get_fundraiser**: Get details of a specific peer-to-peer fundraiser
- **get_person**: Get details of a specific person (donor)
- **get_subscription**: Get details of a specific recurring donation (subscription)
- **list_campaigns**: Campaigns are the primary way to organize fundraising efforts.

List campaigns for the Donately account
- **list_donations**: Useful to track incoming contributions and donor activities. Supports pagination and filtering.

List donations for the Donately account
- **list_fundraisers**: List peer-to-peer fundraisers for the Donately account
- **list_people**: List people (donors/contacts) for the Donately account
- **list_subscriptions**: List recurring donations (subscriptions) for the Donately account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donately** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent donations from Donately."

**🤖 AI Agent:**
> Here are your most recent donations...

---

**👤 You:**
> "Find details about a specific campaign."

**🤖 AI Agent:**
> I found the following details for your campaign...

---

**👤 You:**
> "Retrieve a list of our recurring subscriptions."

**🤖 AI Agent:**
> Here is the list of active recurring subscriptions...


## Installation & Usage

To install and use the **Donately** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donately-alternative](https://vinkius.com/mcp/donately-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

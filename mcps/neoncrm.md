# NeonCRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neoncrm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/neoncrm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/neoncrm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage non-profit operations via NeonCRM — track donations, memberships, and events directly from your AI agent.

## Description
Connect your **NeonCRM** account to your AI agent and take full control of your non-profit organization's constituent data and fundraising activities through natural conversation.

### What you can do

- **Constituent Management** — List all accounts and contacts to get detailed profiles and historical activity.
- **Donation Tracking** — Access a history of all financial contributions and retrieve metadata for specific donations.
- **Membership Oversight** — Monitor active and historical membership records for your supporters.
- **Event Management** — View all organization events (fundraisers, galas) and registration details.
- **Grant Tracking** — List and inspect grant applications and awards managed within the CRM.
- **Custom Data Access** — Retrieve all standard and custom data fields defined for your CRM profiles.

### How it works

1. Subscribe to this server
2. Enter your NeonCRM Organization ID and API Key
3. Start managing your organization from Claude, Cursor, or any MCP client

### Who is this for?

- **Non-Profit Directors** — quickly check fundraising progress or event details without opening the CRM.
- **Development Teams** — verify donor information and membership statuses during outreach.
- **Operations Managers** — automate the retrieval of grant and constituent lists for reporting.


## Available Tools
- **get_account**: Get specific account details
- **get_donation**: Get donation details
- **get_crm_event**: Get specific event details
- **list_accounts**: List NeonCRM accounts
- **list_contacts**: List CRM contacts
- **list_custom_fields**: List CRM custom fields
- **list_donations**: List all donations
- **list_crm_events**: ) created in NeonCRM.

List CRM events
- **list_grants**: List grant records
- **list_memberships**: List account memberships


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NeonCRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all donations received this year."

**🤖 AI Agent:**
> I've retrieved the donation history for this year. You have 45 contributions totaling $12,450.00. The largest single donation was $1,500.00 from 'Global Impact Foundation'. Would you like the details for that specific donation?

---

**👤 You:**
> "Show me the details for account ID 987."

**🤖 AI Agent:**
> Inspecting account 987... This belongs to 'Jane Smith'. She is a 'Gold Member', has been a constituent since 2018, and has a total lifetime giving of $5,600.00. Shall I list her recent event registrations?

---

**👤 You:**
> "List all upcoming CRM events."

**🤖 AI Agent:**
> Retrieving events... You have 3 upcoming events: 'Annual Spring Gala' (Scheduled: May 15th), 'Community Fun Run' (Scheduled: June 2nd), and 'Quarterly Board Meeting'. Would you like to see the registration list for the Spring Gala?


## Installation & Usage

To install and use the **NeonCRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neoncrm](https://vinkius.com/mcp/neoncrm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

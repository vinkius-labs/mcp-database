# Iterable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iterable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iterable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iterable-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage cross-channel marketing campaigns, users, and templates via Iterable API.

## Description
Empower your AI agents to manage your cross-channel marketing with Iterable. This MCP server allows you to list campaigns, retrieve user profiles, track engagement metrics, manage contact lists, and view message templates directly through the Iterable API. Ideal for automating growth marketing and customer lifecycle management.


## Available Tools
- **get_campaign**: Returns message content, audience targeting, and scheduling settings. Use this to analyze the setup of a specific campaign.

Retrieves details for a specific campaign
- **get_campaign_metrics**: Essential for reporting on marketing ROI and audience engagement.

Retrieves performance metrics for a specific campaign
- **get_user**: Essential for deep intelligence on an individual subscriber.

Retrieves details for a user by email
- **list_campaigns**: Returns campaign names, IDs, and statuses. Use this to identify active outreach efforts or locate a specific campaign ID.

Lists all marketing campaigns
- **list_channels**: g., Marketing, Transactional). Essential for understanding the available paths for reaching users.

Lists all communication channels
- **list_lists**: Useful for identifying segments and groups of users for targeted messaging.

Lists all contact lists
- **list_message_types**: g., "Weekly Newsletter", "Welcome Email") defined in the account. Useful for auditing message categorization.

Lists all message types
- **list_templates**: ) available in the account. Useful for identifying content assets used in campaigns.

Lists all message templates
- **list_webhooks**: Useful for auditing system integrations and data exports.

Lists all configured webhooks
- **list_workflows**: Useful for monitoring automated marketing logic and identifying trigger-based campaigns.

Lists all automation workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Iterable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in my Iterable account."

**🤖 AI Agent:**
> I'll fetch the list of your active campaigns from Iterable.

---

**👤 You:**
> "Show me the details for user 'customer@example.com'."

**🤖 AI Agent:**
> I'll retrieve the profile and activity history for that user from Iterable.

---

**👤 You:**
> "Check the metrics for campaign ID '123'."

**🤖 AI Agent:**
> I'll look up the performance metrics and engagement data for that specific campaign.


## Installation & Usage

To install and use the **Iterable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iterable](https://vinkius.com/mcp/iterable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

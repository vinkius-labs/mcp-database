# Joomag MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/joomag)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/joomag-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/joomag-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage digital publications, issues, and analytics via Joomag API.

## Description
Empower your AI agents with Joomag's digital publishing platform. This MCP server allows you to list and retrieve publications, manage issues and collections, track marketing campaigns, and view audience analytics directly through the Joomag API. Ideal for automating content distribution and engagement tracking.


## Available Tools
- **get_account**: Useful for system health checks or verifying access.

Retrieves Joomag account details
- **get_issue**: Use this for deep-dive analysis of a specific edition.

Retrieves details for a specific issue
- **get_publication**: Returns metadata, branding settings, and access configurations. Use this to understand the high-level setup of a digital publication.

Retrieves details for a specific publication
- **list_analytics**: Use this to give the user a status update on overall content performance, views, and engagement trends.

Lists analytics reports for the account
- **list_campaigns**: Useful for monitoring content distribution efforts and identifying which campaigns are driving traffic to publications.

Lists all Joomag marketing campaigns
- **list_collections**: Useful for hierarchical organization or identifying thematic groupings of content.

Lists all publication collections
- **list_contacts**: Includes names, emails, and subscription status. Use this when the user needs to manage or audit the audience list.

Lists all contacts in Joomag CRM
- **list_issues**: Each issue represents a specific version or date-based release. Use this when the user wants to see the content history or find a specific issue ID for a magazine or catalog.

Lists all issues associated with a specific publication
- **list_publications**: Returns publication titles, IDs, and basic settings. Use this to identify which publications are available for further issue management or analytics.

Lists all Joomag publications
- **list_subscriptions**: Use this to audit paying or registered users who have access to restricted content.

Lists all active subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Joomag** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my digital publications in Joomag."

**🤖 AI Agent:**
> I'll fetch the list of your digital publications for you.

---

**👤 You:**
> "Show me the issues for publication ID '456'."

**🤖 AI Agent:**
> I'll retrieve all issues associated with that specific publication.

---

**👤 You:**
> "Check the latest audience analytics report."

**🤖 AI Agent:**
> I'll look up the performance analytics for your Joomag account.


## Installation & Usage

To install and use the **Joomag** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/joomag](https://vinkius.com/mcp/joomag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

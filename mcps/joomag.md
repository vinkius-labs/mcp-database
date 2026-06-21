# Joomag MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/joomag)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage digital publications, issues, and analytics via Joomag API.

## Description
Empower your AI agents with Joomag's digital publishing platform. This MCP server allows you to list and retrieve publications, manage issues and collections, track marketing campaigns, and view audience analytics directly through the Joomag API. Ideal for automating content distribution and engagement tracking.


## Available Tools (10)
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


## ❓ FAQ

**Q: How do I get Joomag API credentials?**
Log in to your Joomag account, navigate to API Settings, and generate a new Access Token.

**Q: Can I see issue details?**
Yes, you can list all issues for a publication and retrieve detailed information for any specific issue.

**Q: Does it support audience analytics?**
Yes, the list_analytics tool provides access to reports and data regarding your publication's performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/joomag](https://vinkius.com/mcp/joomag)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Joomag** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `joomag` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Joomag** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "joomag": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

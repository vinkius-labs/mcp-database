# Craft CMS (Craftnet) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/craft-cms-craftnet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage plugins, licenses, and sales directly via the Craftnet (Craft CMS) API.

## Description
Integrate **Craftnet**, the developer services platform for Craft CMS, directly into your AI workflow. Manage your published plugins, audit CMS and plugin licenses, and track your developer sales using natural language.

### What you can do

- **Plugin Management** — List and retrieve details for all plugins published on the Craft Store.
- **License Auditing** — Monitor Craft CMS and plugin licenses associated with your account.
- **Sales & Payouts** — Track recent sales transactions and historical payout data for your developer profile.
- **Account Insights** — Access metadata for your Craftnet account and explore plugin categories.

### How it works

1. Connect the Craftnet integration to your AI assistant.
2. Authorize using your Craftnet API Key (found in your ID settings at craftcms.com).
3. Manage your Craft CMS ecosystem through intuitive conversation.

### Who is this for?

- **Craft CMS Developers** — Monitor plugin performance and manage licenses without leaving the chat.
- **Agency Owners** — Audit client licenses and track agency-wide plugin purchases efficiently.
- **Digital Marketers** — Search for new plugins and explore store categories during project planning.


## Available Tools (10)
- **get_account_details**: Retrieve metadata for your Craftnet account
- **get_plugin_details**: Get detailed information for a specific plugin
- **list_plugin_categories**: List all plugin categories on the Craft Store
- **list_cms_licenses**: List all Craft CMS licenses in your account
- **list_payout_history**: List historical payouts for plugin developers
- **list_plugin_licenses**: List all plugin licenses purchased or managed
- **list_plugins**: List all plugins published on Craftnet
- **list_sales_history**: List recent sales transactions
- **list_craftnet_users**: List users associated with your Craftnet account
- **search_plugins_by_name**: Search for plugins by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craft CMS (Craftnet)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Craft CMS licenses in my account."

**🤖 AI Agent:**
> I've found 5 Craft CMS licenses. 3 are currently 'Active' and 2 are 'Expired'. Would you like to see the associated domain names for the active ones?

---

**👤 You:**
> "Show me my recent plugin sales for this month."

**🤖 AI Agent:**
> This month you've made 12 plugin sales totaling $450. Your most popular plugin was 'SEOmatic'. Should I list the individual transaction details?

---

**👤 You:**
> "Search for plugins related to 'E-commerce' on Craftnet."

**🤖 AI Agent:**
> I've searched Craftnet and found several e-commerce plugins, including 'Commerce', 'Shopify', and 'Snipcart'. Which one would you like to inspect for details?


## ❓ FAQ

**Q: How do I get a Craftnet API Key?**
Log in to your Craft ID account at craftcms.com, go to **Settings > API Keys**, and generate a new key. Note that some endpoints require developer permissions.

**Q: Can I manage client licenses via chat?**
Yes, you can list all CMS and plugin licenses associated with your account, helping you audit and track renewals or project-specific assignments.

**Q: Does the integration track plugin sales?**
Yes, if you are a plugin developer, you can list your recent sales history and historical payout data directly through the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/craft-cms-craftnet](https://vinkius.com/mcp/craft-cms-craftnet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craft CMS (Craftnet)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `craft-cms-craftnet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craft CMS (Craftnet)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craft-cms-craftnet": {
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
